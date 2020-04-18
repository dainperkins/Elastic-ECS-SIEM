# Elastic-ECS-SIEM
Configs and snippets for Elastic SIEM / ECS 

## Overview
If you happened to see the Elastic SIEM / ECS Webinar this is the spot where I'll 
be dropping various configs, code chunks, links, etc. for Elastic ECS SIEM integration
with various network / security logging formats.

### ASA
This folder contains a quick logstash config to parse out local ASA Login Messages, ecs
compliant and integrates wiht Elastic SIEM functionality.

### Meraki
This folder contains Logstash pipelines for handling Meraki syslogs, as well as logstash
configs for pulling asset information from the Meraki Dashboard API, an enrichment policy, 
and an Elastic ingest pipeline for handling geoip, asn, and meraki asset enrichment for
observers (when Meraki devices are reporting as observers) and hosts (for e.g. 1x login)
etc.)