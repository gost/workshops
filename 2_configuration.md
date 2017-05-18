# 2] GOST configuration

## Introduction

Now that GOST is installed let's configure GOST with some metadata about our sensors.

## Prerequisites

- Postman

Verify that Postman is installed. If not, download it from https://www.getpostman.com/

If installed, open the file 'SensorThings API v1.0.postman_collection.json'

After import, Postman should look like:

<img src = "images/postman.png">

## Create items

Use the Postman file to send the following requests:

- Step 1: Create a Thing

- Step 2: Create an ObservedProperty

- Step 3: Create a Sensor

- Step 4: Create a Datastream 

- Step 5: Create an Observation

Note: In step 1, 2, 3 make a note of the iot.id created, you'll need these id's in step 4 and 5 to replace 'id_of_the_entity_you_just_created' parameter.

## Testing

Open http://localhost:8080 and browse through the various entities

