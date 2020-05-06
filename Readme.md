Cloud DevOps Engineer Capstone Project

In this project, I applied my skills and knowledge which was developed throughout the Cloud DevOps Nanodegree program.

## Project Tasks:

* Working in AWS
* Using Jenkins to implement Continuous Integration and Continuous Deployment
* Building pipelines
* Working with CloudFormation to deploy clusters
* Building Kubernetes clusters
* Building Docker containers in pipelines

## About Project: 

> I created a CI/CD pipeline to use Blue/Green Deployment to deploy a static website.

## Project Requirement:

> This project requires:

* Jenkins
* Blue Ocean Plugin in Jenkins
* Pipeline-AWS Plugin in Jenkins
* Docker
* Pip
* AWS Cli
* Eksctl
* Kubectl

## The files included are:
```sh
Master Branch
* Jenkinsfile : Jenkinsfile for creating cluster

Deployment Branch
* Jenkinsfile : Jenkinsfile for deploying container
* Dockerfile : Dockerfile for building the image 
* green-controller.json : Create a replication controller green pod
* green-service.json : Create the green service
* blue-controller.json : Create a replication controller blue pod
* blue-service.json : Create the blue service
* index.html : Web site Index file.
```

## Run the project:
```sh
* Run the Master branch files with Jenkins.
* Run the Deploy branch files with Jenkins.
```
