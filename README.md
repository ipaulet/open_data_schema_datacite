# Open Data Schema Map: DCAT-AP
DKAN Module which provides Schema.org-type Metadata (in JSON-LD format) for DataCite ingest and DOI retrieval.

Schema module to provide endpoints for DCAT-AP, the DCAT Application profile for data portals in Europe. The schema provided is in JSON but includes XML prefixes, and is indended primarily for output to XML/RDF.

Two schemas are actually provided:

DCAT Catalog: Can be used to create an entire data catalog, usually in XML format and exposed at /catalog.xml.
DCAT Dataset: Schema for providing a single-dataset endpoint
DKAN's implementation adds meta links in page headers to catalog.xml, and links in each dataset page (as well as header links) to the dataset-specific endpoints.
