# MedCom FHIR starter project


* Clone this project
* Step into the cloned folder
* Run the following: `docker run -p 80:8080 --add-host fhir.medcom.dk:172.20.0.11 -v $(pwd)/configs:/configs -e "--spring.config.location=file:///configs/medcom-core-v0.9.yaml" hapiproject/hapi:latest`
* Done!




# Modifying the templates using an exploded version of the HAPI FHIR starter project

1) Build the docker image with the provided Dockerfile (eg. ```docker build . --no-cache -t medcom ```).
2) Start the docker container by eg: ```docker run -p 80:8080 --add-host fhir.medcom.dk:172.20.0.11 -v $(pwd)/configs:/configs -e "--spring.config.location=file:///configs/medcom-core-v0.9.yaml" medcom```
3) Enjoy!
