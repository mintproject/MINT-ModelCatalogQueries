# Queries for Mint-ModelCatalog Endpoint

This document separates a set of interesting queries that are useful to explore the model catalog.

These queries are exposed as a REST API through the GRLC (garlic) application.

SPARQL Endpoint for the model catalog available at: http://ontosoft.isi.edu:3030/dataset.html

GRLC REST API documentation available at: http://ontosoft.isi.edu:8001/api/KnowledgeCaptureAndDiscovery/KnowledgeCaptureAndDiscovery/MINT-ModelCatalogQueries

GRLC REST APU spec available at: http://ontosoft.isi.edu:8001/api/KnowledgeCaptureAndDiscovery/KnowledgeCaptureAndDiscovery/MINT-ModelCatalogQueries/spec




-----------------

List of queries to be implemented:

(done) getModels 
    returns description, label, category, versions.
    
(done) getVersion<version> (done by adding a generic getResourceMetadata<URI>)
    given a version, returns all the metadata about it.

getConfigurations
    returns version, configuration, description, other metadata such as invocation code.
    
getConfiguration<config> (done by adding a generic getResourceMetadata<URI>)
    returns all the metadata about <config>: version, configuration, description, other metadata such as invocation code.
    
getVariablePresentationsForModel<Model>
    returns configuration, input variables, output variables

getConfigurationsI_O
    returns configurations, inputs files, output files.
    
getInputForStandardVariable<Variable>
    returns the input (or output) for the standard variable provided 
    
getModelsForCategory <string:Category>
    returns the models associated to a particular category

getVariablesAndUnits<Input/Output>
    returns the variablePresentations associated to the provided input/output, and their units.


