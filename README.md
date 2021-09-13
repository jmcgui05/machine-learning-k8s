# machine-learning-k8s

[![jmcgui05](https://circleci.com/gh/jmcgui05/machine-learning-k8s.svg?style=svg)](https://app.circleci.com/pipelines/github/jmcgui05/machine-learning-k8s?branch=main)

A Machine Learning Microservice that uses Docker and Kubernetes for Containerization. To run it locally, simply run `python app.py`

## Project Details

**app.py** is a simple Python file that runs predictiosnand prints required json data to the terminal

**Dockerfile** is a standard docker file that containerizes the app.py and runs it

**make_prediction.sh** is a simple helper script that will hit your local service and run predictions

**Makefile** is a standard make file that will run setup, install, lint and tests for your app

**requirements.txt** is a simple text file containing the libraries your app needs, and is used in the Makefile during install

**run_docker.sh** is a simple script to build and run your Docker container

**update_docker.sh** is a simple script that will tag a docker image and push it to docker hub

**run_kubernetes.sh** is a simple script that will set your docker path, create a deployment and forward ports