These are the API pollers for the meraki device info, all you need is the api key (get it from the dashboard) and put it in the Logstash leystore and you are good to go.

The Meraki .9 API is goofy, and while its a little annoying, the pollers start from organization every time, so any updates will be picked up (new org,new devices, etc.) without having to do anything.

That being said this is probably not the most api / programmatically efficient way of getting this done, but it works.