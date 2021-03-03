#Final Project

This case study extends the CI/CD Pipeline Project with provisioning and monitoring components. 

In this project the steps that I followed are:
 
* Create a Jenkins(CI/CD) pipeline to deploy a Flask application onto a Kubernetes cluster created with Ansible.
* Install and configure monitoring of your Kubernetes clusters and Flask application.
* Use Prometheus/Grafana to monitor the cluster  
* Create a load with a tool like stress to simulate application activity. 

##Project Milestones

###Stage One: 

Project Desing

<img src"./Pictures/Final.pdf">

List of components in the architecture:

* GitHub
* Docker
* Jenkins
* Kubernetes (minikube)
* Prometheus/Grafana

###Stage Two:

Deployment

* Minikube start the cluster locally

<img src"./Pictures/minikube.pdf">

* Deploy the Flask application in the cluster using Ansible

<img src"./Pictures/jenkins.pdf">

* Check if the app is running

<img src"./Pictures/service.pdf">

<img src"./Pictures/app.pdf">

###Stage Three:

Monitoring

* Donwload Prometheus/Grafana using Helm

* By installing with Helm automaticaly will setup Prometheus/Grafana for us

<img src"./Pictures/cluster.pdf">

* Port-forward the grafana pod to show the Dashboard on the browser in port 3000

<img src"./Pictures/dashboard.pdf">

* Get the minikube cluster information

<img src"./Pictures/metric1.pdf">

<img src"./Pictures/metric2.pdf">

<img src"./Pictures/metric3.pdf">

* Get the information of the application pod

<img src"./Pictures/pod.pdf">

* Stress the port where the applications is and see the difference

<img src"./Pictures/stress.pdf">

<img src"./Pictures/stress2.pdf">