# Queries for Mint-ModelCatalog Endpoint

This document separates a set of interesting queries that are useful to explore the model catalog.

These queries are exposed as a REST API through the GRLC (garlic) application.

SPARQL Endpoint for the model catalog available at: http://ontosoft.isi.edu:3030/dataset.html

GRLC REST API documentation available at: http://ontosoft.isi.edu:8001/api/KnowledgeCaptureAndDiscovery/MINT-ModelCatalogQueries

GRLC REST APU spec available at: http://ontosoft.isi.edu:8001/api/KnowledgeCaptureAndDiscovery/MINT-ModelCatalogQueries/spec




-----------------

# List of queries to be implemented:

* (done) getModels: returns a description, label, category and versions of each model.  
* (done) getResourceMetadata [iri:URI]: given a resource (model, version, configuration, etc.), returns all the metadata about it.
* getConfigurations: returns version, configuration, description, other metadata such as invocation code.
* getVariablePresentationsForModel[iri:Model]: returns a list of the available configurations, input variables and output variables given a certain model
* getConfigurationsI_O: returns a list of configurations, their inputs files and output files.
* getInputForStandardVariable[string:Variable]: returns the input (or output) for the standard variable provided 
* getModelsForCategory (string:Category]: returns the models associated to a particular category
* getVariablesAndUnits[iri:Input/Output]: returns the variablePresentations associated to the provided input/output, and their units.
* getModelOutputsForVariable [string:standard name]: Query that given a standard variable, returns the models which produce output variables with a particular standard name (or canonical name)
* getCAG: Given a model configuration, return the list of processes being modeled and how they influence each other. 



