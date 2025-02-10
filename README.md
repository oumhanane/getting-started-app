# Getting started

This repository is a sample application for users following the getting started guide at https://docs.docker.com/get-started/.

The application is based on the application from the getting started tutorial at https://github.com/docker/getting-started

Cloning the project: I cloned the "getting-started-app" project from the repository to work on the application in a Kubernetes environment.

Creating the Dockerfile: I wrote a Dockerfile to build the Docker image for the application. This file includes instructions to define the base image (here, node:18-alpine), add the project files, and install dependencies using the yarn install command.

Creating and deploying the pod on Kubernetes: I used Minikube to set up a local Kubernetes cluster. I created a Kubernetes deployment file (mon_appli_oc.yaml) with the necessary specifications, replacing the Docker image with the one built from the Dockerfile. I also created a service file (mon_appli_oc_service.yaml) to expose the application and allow external access. I then applied these configuration files to Kubernetes and confirmed that the pod started correctly, along with the service.