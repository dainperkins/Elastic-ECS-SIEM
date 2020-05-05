## Elasticsearch stuff for meraki

the asset mapping is a slightly tweaked ECS with host/observer fields at the top level for easy enrichment
into appropriate fields. (e.g. name -> host.name, ip -> host.ip, geo -> observer.geo, etc.)


* meraki-asset-index-mapping.json. - index mapping for Meraki assets, slightly tweaked from ECS to avoid renames in enrichment process
* meraki-host-enrich.json	es  - host fields enrichment processor
* meraki-ingest-pipeline-7_7.json - meraki ingest pipeline
* meraki-observer-enrich.json	- observer fields enrichment processor
* template_ecs-asset.json - index template for asset db
