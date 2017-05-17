# 1) GOST installation

# Introduction

In this page installation of GOST is described using Docker.

## Prerequisites

Verify that Docker is installed:

```
$ docker --version
Docker version 17.05.0-ce, build 89658be
$ docker-compose --version
docker-compose version 1.13.0, build 1719ceb
```

If Docker is missing, install it for <a href="https://docs.docker.com/docker-for-mac/install/#download-docker-for-mac">Mac</a> or <A href="https://docs.docker.com/docker-for-windows/install/">Windows</a>

## Installation

Installation if GOST is easy: download the docker-compose file and run it.

```
$ https://raw.githubusercontent.com/Geodan/gost/master/src/docker-compose.yml
$ docker-compose up
```

## Testing

Open a browser and test the following addresses:

- http://localhost:8080 : should run the dashboard

- http://localhost:8080/v1.0: should run the GOST endpoint

- http://localhost:1880 : should run Node-RED







