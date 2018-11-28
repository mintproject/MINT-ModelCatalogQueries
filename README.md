# Queries for Mint-ModelCatalog Endpoint

This document separates a set of interesting queries that are useful to explore the model catalog.

These queries are exposed as a REST API through the GRLC (garlic) application.

SPARQL Endpoint for the model catalog available at: http://ontosoft.isi.edu:3030/dataset.html

GRLC REST API documentation available at: http://ontosoft.isi.edu:8001/api/KnowledgeCaptureAndDiscovery/MINT-ModelCatalogQueries

GRLC REST APU spec available at: http://ontosoft.isi.edu:8001/api/KnowledgeCaptureAndDiscovery/MINT-ModelCatalogQueries/spec




-----------------

# List of queries supported by the API:

* (done) getConfigI_OVariablesAndStandardNames[iri:ModelConfiguration]: Given a model configuration URI, this query returns the inputs/outputs and their corresponding variable presentations and standard names.
* (done) getI_OForStandardVariable[string:Variable]: Given a standard name, this query returns which input, output, configuration, version and model refers to it.
* (done) getI_OVariablesAndUnits[iri:Input/Output]: returns the variablePresentations associated to the provided input/output, and their units.
* (done) getModelCategories: Query that returns all available model categories.
* getModelConfigurationMetadata [iri:Configuration URI]: Returns all metadata of a configuration: the model version it belongs to, its label, description, inputs, outputs, modules, processes, time step (unit and value) and CAG id associated to it.
* (done) getModelConfigurations: returns all existing configurations, the model and model version they belong to, their label and description associated to them.
* (done) getModelConfigurationsI_O: Returns a list of all available configurations, their inputs files and output files.
* (done) getModelConfigurationsForVariable [string:standard name]: Query that given a standard variable, returns the model configurations which produce output variables with that standard name. 
* (done) getModels: returns a description, label, category and versions of each model.  
* (done) getModelsForCategory (string:Category]: returns the models associated to a particular category
* (done) getProcessesForCAG[iri:CAG]: Given a CAG, return all the processes associated with it (and their dependencies).
* (done) getResourceMetadata [iri:URI]: given a resource URI (model, version, configuration, etc.), returns all the metadata about it.
* (done) getVariablePresentationsForModel[iri:Model]: returns a list of the available configurations, input variables and output variables given a certain model

 
 



