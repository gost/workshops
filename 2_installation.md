# 2) GOST installation

# Introduction

In this page installation of GOST is described using Docker.

## Prerequisites

Verify that Docker is installed with command 'docker info'. This command should display system-wide Docker information.

```
$ docker info
Containers: 250
 Running: 0
 Paused: 0
 Stopped: 250
Images: 1062
...
```

Run command 'docker-compose -- version', version should be 1.10 or greater:

```
$ docker-compose --version
docker-compose version 1.13.0, build 1719ceb
```

If Docker is missing, install it for <a href="https://docs.docker.com/docker-for-mac/install/#download-docker-for-mac">Mac</a> or <A href="https://docs.docker.com/docker-for-windows/install/">Windows</a>.

Note: If you use VirtualBox on Windows be sure to switch it off https://derekgusoff.wordpress.com/2012/09/05/run-hyper-v-and-virtualbox-on-the-same-machine/

If you are unable to install Docker, you can try the free online service <a href="http://labs.play-with-docker.com/">play-with-docker</a>, it gives you free Docker machines for 4 hours.

## Installation

Installation of GOST is easy: download the docker-compose file and run it.

Note: The first time the 'docker-compose up' command is executed, a bunch of new Docker images will be downloaded and started 
so please be patient.

```
$ curl https://raw.githubusercontent.com/gost/docker-compose/master/docker-compose.yml > docker-compose.yml
$ docker-compose up
```
The system is ready when log messages appear like:

```
gost_1       | 2017/06/26 09:49:21 Started GOST HTTP Server on :8080
node-red_1   | 26 Jun 09:49:23 - [info] Started flows
gost-db_1    | LOG:  database system is ready to accept connections
mosquitto_1  | 1499082438: New client connected from 172.18.0.5 as gost (c1, k300).
```

## Testing

Open a browser and test the following addresses:

- http://localhost:8080 : should run the dashboard

- http://localhost:8080/v1.0: should run the GOST endpoint

- http://localhost:1880 : should run Node-RED user interface

Continue to <a href="3_configuration.md">3) GOST Configuration</a>

