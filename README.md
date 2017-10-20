# jenkins
A Jenkins image with pre-installed Java 8, Maven and Git

## Contents
This Jenkins image has the following:
- Latest Jenkins LTS
- OpenJDK 8
- Maven 3
- Nano
- Git
- Minimal plugins to get CI process started

## Pre-installed Jenkins plugins
- Maven Integration
- Docker and Docker Slaves
- Build Pipeline
- Config File Provider
- Console Column
- Copy to Slave
- Extra Columns
- Favorite
- Folder
- Git
- HTML Publisher
- Javadoc
- Workflow Aggregator
- Docker Build Step

## Build from Dockerfile
1. Run command: `docker build -t thetestguys/jenkins .`

## How to run
1. Pull the docker image: `docker pull thetestguys/jenkins`
2. Run with this command: `docker run -d thetestguys/jenkins`

## Additionals
* Notice that plugins.txt should not have any empty line at the end of file (especially when building in Windows)
* Included is a docker-compose.yml which starts up this Jenkins image and a Selenium Grid setup (a hub, a Firefox node and a Chrome node)
