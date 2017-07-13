# 3] GOST configuration

## Introduction

Now that GOST is installed let's configure GOST with some metadata about our sensors.

## Prerequisites

- Postman

Verify that Postman is installed. If not, download it from https://www.getpostman.com/

If installed, import the file <a href="SensorThings API v1.0.postman_collection.json">SensorThings API v1.0.postman_collection.json</a> from this workshop repository.

In Postman, click the 'Import' button, click Import from link, using url 'https://raw.githubusercontent.com/gost/workshops/master/2017_foss4g_boston/SensorThings%20API%20v1.0.postman_collection.json' and press 'Import'

<img src = "images/postman_import.png">

After import, Postman should look like:

<img src = "images/postman.png">

## Create items

With Postman, we can easily send HTTP requests to the GOST server. On the left panel, select a request ('Step 1: Post a Thing'), on the right panel press 'Body' and Request body text will show up. After hitting 'Send' button the HTTP Response will be showed below the request.  

Use the Postman file to send the following requests, be sure to inspect the request and response to see whats going on:

- Step 1: Create a Thing

- Step 2: Create an ObservedProperty

- Step 3: Create a Sensor

- Step 4: Create a Datastream 

- Step 5: Create an Observation

Note: In step 1, 2, 3 make a note of the iot.id created, you'll need these id's in step 4 and 5 to replace 'id_of_the_entity_you_just_created' parameter. The first item created will have number 1 by default, so use that in most cases.  

## Testing

Open the dashboard http://localhost:8080 and browse through the various entities (Things, ObervedProperties, Sensors, Datastreams, Observations) and check if your data is there.

<img src = "images/dashboard.png"/>

Continue to <a href = "4_nodered.md">4) GOST and Node-RED</a>

