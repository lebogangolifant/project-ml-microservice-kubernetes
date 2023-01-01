[![CircleCI](https://dl.circleci.com/status-badge/img/gh/lebogangolifant/project-ml-microservice-kubernetes/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/lebogangolifant/project-ml-microservice-kubernetes/tree/main)

## Machine Learning Microservice API, using kubernetes.

### Project Overview
This project, operationalize a Machine Learning Microservice API, contains a pre-trained, sklearn model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on the data source site. This project tests out predictions (inference) about housing prices through API calls.

### Project Function:
* Run a Docker Container & Make a Prediction
* Upload your Docker image into a public registry 
* Run deployed application in a Kubernetes cluster
* Automated environment testing with CircleCI

### Instructions:
* Requirements
 - `Python 3.7`

* Fork repo & clone repo

## Install dependencies:

### Set up the environment:
* create a virtual environment in your home directory called .devops
 - Run `make setup`

### Install dependencies:
 - Run `make install`
 - (Optionally) Lint application (requires hadolint)

### Run Docker container:
* Run the application on docker by calling `./run_docker.sh`

### Upload to Docker Hub:
* In the `./upload_docker.sh` file, edit the dockerpath, change the docker username to a personalized one (or leave it as is, to use the public webdevprojects/microserviceproject:v1.0.0)

### Upload to docker hub:
* Run `./upload_docker.sh`

### Deploy Kubernetes:
* Run `./run_kubernetes.sh`