# Getting started

This repository is a sample application for users following the getting started guide at https://docs.docker.com/get-started/.

The application is based on the application from the getting started tutorial at https://github.com/docker/getting-started

Cloning the project : I cloned the project "getting-started-app" from the repository to work on the application in a Kubernetes environment.

Creating the Dockerfile : I wrote a Dockerfile to build the Docker image for the application. This file includes instructions to define the base image (here, node:18-alpine), add the project files, and install dependencies using yarn install.

Creating and deploying the pod on Kubernetes : I used Minikube to set up a local Kubernetes cluster.
I created a Kubernetes deployment file (deployment.yaml) using the minikube kubectl -- create deployment command, specifying the Docker image (mon_image) built from the Dockerfile.
I then applied this deployment on Kubernetes and confirmed that the pod started correctly.