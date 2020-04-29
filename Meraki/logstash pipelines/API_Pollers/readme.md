These are the API pollers for the meraki device info, all you need is the api key (get it from the dashboard) and put it in the Logstash leystore and you are good to go. {meraki_api}

Replace the other ${} variables, or define in the logstash keystore as you prefer: 
  ip, port for the syslog input
  elastic host, username, password.

The Meraki .9 API is goofy, and while its a little annoying, the pollers start from organization every time, so any updates will be picked up (new org,new devices, etc.) without having to do anything.

That being said this is probably not the most api / programmatically efficient way of getting this done, but it works.

The ingest pipeline includes some enrichments (meraki host for eap authentications, and meraki observers for everything else coming in via syslog).

The Elasticsearch directory has that info, formatted to just drop into the dev console.
