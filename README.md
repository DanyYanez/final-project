# Final Project

This case study extends the CI/CD Pipeline Project with provisioning and monitoring components. 

In this project the steps that I followed are:
 
* Create a Jenkins(CI/CD) pipeline to deploy a Flask application onto a Kubernetes cluster created with Ansible.
* Install and configure monitoring on the Kubernetes clusters and Flask application.
* Use Prometheus/Grafana to monitor the cluster  
* Create a load with a tool like stress to simulate application activity. 

## Project Milestones

### Stage One: 

Project Desing


<img src="./Pictures/Final.png">

List of components in the architecture:

* GitHub
* Docker
* Jenkins
* Kubernetes (minikube)
* Prometheus/Grafana

### Stage Two:

Deployment

* Minikube will start the cluster locally

<img src="./Pictures/minikube.png">

* Deploy the Flask application in the cluster using Ansible

<img src="./Pictures/jenkins.png">

* Check if the app is running

<img src="./Pictures/service.png">

<img src="./Pictures/app.png">

### Stage Three:

Monitoring

* Download Prometheus/Grafana using Helm

* Installing Prometheus/Grafana with Helm will automatically set it up

<img src="./Pictures/cluster.png">

* Port-forward the grafana pod to show the Dashboard on the browser in port 3000

<img src="./Pictures/dashboard.png">

* Get the minikube cluster information

<img src="./Pictures/metric1.png">

<img src="./Pictures/metric2.png">

<img src="./Pictures/metric3.png">

* Get the information of the application pod

<img src="./Pictures/pod.png">

* Stress the port where the applications is and see the difference

<img src="./Pictures/stress.png">

<img src="./Pictures/stress2.png">

<img src="./Pictures/stress4.png">

<img src="./Pictures/stress3.png">
