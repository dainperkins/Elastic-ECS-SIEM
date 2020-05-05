## Elasticsearch stuff for meraki

the asset mapping is a slightly tweaked ECS with host/observer fields at the top level for easy enrichment
into appropriate fields. (e.g. name -> host.name, ip -> host.ip, geo -> observer.geo, etc.)
