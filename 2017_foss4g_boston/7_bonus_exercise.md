# 7] Bonus exercise

Exercise: Real-time mapping Boston bike stations with GOST - 
where are bikes available? 

Station information: https://gbfs.thehubway.com/gbfs/en/station_information.json
Availablility per station: https://gbfs.thehubway.com/gbfs/en/station_status.json

Tasks:

1] Initialize datastreams

Make a Node-RED flow to create a Datastream per bike station. Run this flow 1 time.

2] Get data

Read https://gbfs.thehubway.com/gbfs/en/station_status.json each minute and create the correct 
observations per bike station.

3] Visualize in Map

Create a map (OpenLayers or Leaflet) with real-time bike station information.





