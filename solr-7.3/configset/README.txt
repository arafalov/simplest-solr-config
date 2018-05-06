Uses id field, set as uniqueId to allow reindexing the data. 

All data is assumed single-valued as multi-valued data often needs to be configured explicitly and therefore the schema may be configured as well.

The new SortableTextField means the data can be searched as a normal text field and also sorted/faceted on the full original string.

Everything is copyFielded into the _text_ field (_text_ to match newer Solr conventions) and is therefore a good baseline field to search before adding relevance-tuning queries.
