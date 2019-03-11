# Open Data Schema Map: DataCite
DKAN Module which provides Schema.org-type Metadata (in JSON-LD format) for DataCite ingest and DOI retrieval.

Schema module provide Schema.org endpoints for later import in DataCite. DataCite offers support for schema.org in JSON-LD format to DOI content negotiation. With this module the Schema.org metadata can be embedded using JSON-LD and is intended for further use in generating the DataCite DOI and asociated metadata schema. As presented in this article: Using Schema.org for DOI Registration (https://doi.org/10.5438/0000-00cc), we use the DataCite posibility of ingesting different types of file-format in order to bring the DKAN Dateset mapped fields into a DataCite XML Metadata Schema.

This schema follows the  machine-readable format of Schema.org and displays single-dataset endpoint. This is a submodule of the main module ODSM (Open Data Schema Map) and has the open_data_schema_ckan module as a model - as recommended in the "Adding new schemas" section of DKAN Documentation (https://docs.getdkan.com/en/latest/components/open-data-schema.html?highlight=odsm).

### Instalation:

Copy the downloaded folder of the open_data_schema_datacite submodule in the ODSM/module/ folder structure.
Enable the main Open Data Schema Map module as usual, and enable the "DataCite" schema module we will need to create our API.

### Create new API:

Navigate to admin/config/services/odsm and click "Add API."
Here we give the API a title, machine name, choose the node entity type and dataset bundle. As endpoint we define a new, custom one: 
api/3/action/package_show_datacite. Afterwards we check the "Enabled" field and choose the "json-pretty" output format and the "DataCite Dataset" schema.

