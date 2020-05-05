## Elasticsearch stuff for meraki

enrichment, index mapping, and ingest pipeline used with the Meraki logstash pipelines


* meraki-asset-index-mapping.json. - index mapping for Meraki assets, slightly tweaked from ECS to avoid renames in enrichment process
* meraki-host-enrich.json	es  - host fields enrichment processor
* meraki-ingest-pipeline-7_7.json - meraki ingest pipeline
* meraki-observer-enrich.json	- observer fields enrichment processor
* template_ecs-asset.json - index template for asset db
