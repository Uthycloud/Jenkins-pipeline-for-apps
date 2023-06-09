# Project Name: Microservices-based architecture deployment on Kubernetes using a Jenkins CI/CD Pipeline


This project is a demonstration of how to deploy a microservices-based architecture on Kubernetes using an Infrastructure as Code (IaaC) approach. I provisioned two different webapps- A Socks Shop microservice application and a simple Nginx webpage app with an nginx/httpd frontend proxy and a database backend.

I started by setting up a Jenkins Server first, a well detailed guide on how to go about this and the codes i used are in this my repository below. 

[Check it out here](https://github.com/Uthycloud/Deploy-Jenkins-Server-with-Terraform)

The deployment process is triggered by a deploy pipeline that uses Terraform to provision the kubernetes cluster on AWS. Once the infrastructure is in place, Terraform takes over to deploy the webapp, database, and microservices.

#### Metrics, Monitoring, and Logging
I used Prometheus as the monitoring tool for this project. Prometheus is a powerful and flexible monitoring system that provides real-time metrics and alerts.


#### Setup Details
To recreate this setup, you'll need to provision the following components:

- A webapp of your choosing with an nginx/httpd frontend proxy
- A database backend (mongo, postgresql, etc.)
- The Socks Shop example [microservice application](https://microservices-demo.github.io/)
- Infrastructure as Code

This project emphasizes readability, maintainability, and DevOps methodologies. I've used Terraform as the configuration management tool to automate the deployment process.

