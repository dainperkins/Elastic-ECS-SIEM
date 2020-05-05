This is the full scope of Meraki logstash pipelines.  If you are getting grok errors or something similar open an issue, 
drop the raw message and I'll do my best to update.

The logstash pipelines rely on an ingest pipeline as well as some enrichment processing to get the Meraki observer/host 
information provided.

To do:
+ Client Enrichment - polling api for clients periodically
+ Network Enrichment (e.g. internal subnets) I think this can come from mx info
