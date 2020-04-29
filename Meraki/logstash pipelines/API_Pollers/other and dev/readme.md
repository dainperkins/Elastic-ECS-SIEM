The Amp api logstash pulls AMP / IDS alerts from the Meraki API, the only problem is its from a network perspective, so theres no observer information.

The orgs file is one of the dev config files I used playing with the api, trying to get everything in a single config file, due to the variations in network level, and device level info for SSIDs, and api v.9 not sending lanips for MXs (Meraki support says "expected"... so I suppose theres nothing but just waiting for v1 to be out...)

I suspect the web hook functionality may be easier to deal with as well, tho I wonder how the device/network level annopyances will work, but it requires a public end point, and will probably require the same level of org/network/device enrichment, but we'll see.
