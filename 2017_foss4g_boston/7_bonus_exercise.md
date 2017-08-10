# 7] Bonus exercise

Exercise: Real-time mapping Boston bike stations with GOST - 
where are bikes available? 

Station information: https://gbfs.thehubway.com/gbfs/en/station_information.json

Availablility per station: https://gbfs.thehubway.com/gbfs/en/station_status.json

Stations near workshop: 

* [99]  Harvard University’s Center for Geographic Analysis (CGA). id: 110 
* [187] Verizon Innovation Hub 10 Ware Street. id: 221
* [86]  Cambridge Main Library at Broadway / Trowbridge St. id: 96

Stations near venue:
* [26]  Seaport Hotel - Congress St at Seaport Ln. id: 31
* [57]  Boston Convention and Exhibition Center - Summer St at West Side Dr. id: 65
* [158] Congress St at Northern Ave. id: 186


Tasks:

1] Initialize datastreams

Make a Node-RED flow to create a Datastream per bike station. Run this flow 1 time.

2] Get data

Read https://gbfs.thehubway.com/gbfs/en/station_status.json each minute and create the correct 
observations per bike station.

3] Visualize in Map

Create a map (OpenLayers or Leaflet) with real-time bike station information.

For instance you can use the javascript MQTT library Paho by eclipse to retrieve the location information from Gost, see also https://github.com/gost/docs/blob/master/gost_mqtt_getting_started.md




