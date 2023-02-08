## Containers

This repository has been created to host the development and build (through a CI/CD github action) of the Docker containers used in the VRE. 

The following repositories each build a separate container:
 - `rucio-client` builds the image to use the rucio instance with ESCAPE credentials, to connect tot he rucio instance following the appropriate [documentation](https://datalake-rucio.docs.cern.ch/). 
 
The secret for the action is stored Under Settings/Secrets and variables/Actions. 
The `DOCKER_USER` is `projectescapeservice`.
The `DOCKER_TOKEN` is the token requested from the `projectescapeservice` account (log in to Dockerhub with the password stored in tbag and navigate to Account Settings/Security). 
 
