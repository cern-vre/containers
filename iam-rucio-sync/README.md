## Automatised build of the iam-rucio-sync container

This repository contains the Dockerfile for the IAM Rucio syncronisation enabled for the [ESCAPE](https://projectescape.eu/) VO, used to authenticate users to the VRE. Basic DB operations can also be executed. 

The base image is the Rucio server container 

If you want to change something in the Docker image, you can change the Dockerfile, push the changes to the `main` branch, and the CI/CD workflow will publish the new image on the [ESCAPE DockerHub](https://hub.docker.com/orgs/projectescape/). 

## Rucio-clients version change

Change the Makefile with the desired variables. ASETAG file to your desired most recent version. 

## Build Docker image manually (python 3 by default)

```bash
$ make build
```
Check that the image has been built and tagged successfully with `docker images`. 
Log in to Docker with `docker login`, then:

```bash
$ make push
```
