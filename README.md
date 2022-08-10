[![CircleCI](https://circleci.com/gh/kent2cky/kent2cky-project-ml-microservice-kubernetes.svg?style=svg)](https://app.circleci.com/pipelines/github/kent2cky/kent2cky-project-ml-microservice-kubernetes)

## Project Overview

This project operationalizes a Machine Learning Microservice API using kubernetes. To get this project working one needs to be comfortable working with kubernetes, docker, bash scripts, makefiles and python. 

## In this project we:

- made sure that the app codes are well formatted and running
- checked the code into CircleCI for CI/CD
- containerized our machine learning project using docker
- got the docker container running
- uploaded the docker container my public registry
- created kubernetes pods and clusters using the docker image


## Steps to run

### step 1
- clone this repo into your local machine

### Step 2
- run `make setup` to setup your local environment.
- run `make install` to install all required dependencies.
- run `make lint` to lint the application codes

### Step 3
- run `./run_docker.sh` to containerize and run the application using docker

### Step 4
- the `./upload_docker.sh` file to put in your own dockerpath and then run the script to upload the docker container to your docker hub account`

### Step 5
- run `./run_kubernetes.sh` to get the container running on kubernetes

### Step 6
- sit back relax and enjoy your working application :-).
