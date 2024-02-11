# Data Sandbox

## Purpose
I wanted to provide a sandbox environment in Kubernetes to support API development, and data pipeline management.

## Requirements
docker:^20.10.17    
kubectl:^1.25.4    
minikube:^1.30.1  

## Setup

### Jenkins Configuration
generate ssh permissions for Jenkins worker node(s) (no passphrase)     
./gen-ssh.sh

create .ssh/github-personal-token and paste your github PAT token with repo access

### Minikube Configuration
* minikube start
* docker build jenkins/jenkins-controller .
* minikube image load jenkins/jenkins-controller:latest

### AWS Cloud Configuration
Todo