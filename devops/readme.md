# Tradeling DevOps Challenge

<p align="left">
<a href="https://tradeling.com"><img src="https://c8n.tradeling.com/assets/svgs/tradeling-logo.svg" alt="Tradeling" width="250"/></a>
</p>

## Goal
The challenge goal is to build a fully automated infrastructure and CI/CD solution for a simple web-based application.
We prefer well-thought-out solutions over the quick-and-dirty kind. So take your time, if you need it. A rushed job is usually matched by a swift rejection.

## Context
We have developed a simple "todo" web application, it's inside the /app directory in this repo.
The application main features are:
- Users can sign up / sign in
- Users can manage their Todo list  [ add / edit / list / delete]

The application developed using node.js, and it requires mongoDb database for storing data.

## The Task
The task is to deploy the application on AWS using Kubernetes.
* You shouldn't use any ready K8 setup like EKS/AKS,etc. but for sure you can use any k8 automation tools like kops, kubeSpray, kubeadm,etc.
* Make sure to not have any manual installations rather use configuration managers such as Ansible / Saltstack etc.
* Review your solution and ensure it follows the best practices of building and deploying microservices.
* Prepare a detailed document and/or instructions about what you have done. These documents must detail steps for other DevOps Engineer to understand how to deploy this application and maintain it.

## Instructions
- Using Terraform, build the infrastructure resources such as PVC, subnets, instances, elb, security group, etc., in the most optimal way with Production Grade security measures.
- Build a Kubernetes Cluster in this VPC in an internal subnet, You can use any tool todo this.
- You may need to modify the application source code or configuration in order to make the application running on the Kubernetes cluster, e.g. make use ENV variables in 12Factor style, create Dockerfile.
- You need to update the application dependencies [node modules] to last stable and compilable version, please document how you achieved this part.
- Build the Docker image using GitHub actions / Circle CI / Drone CI etc.
- Build the Kubernetes deployments or Helm charts for the application.
- Deploy the MongoDB on either Kubernetes or EC2 with High Availability mode (master/slave) and configure it with the Application.
- Deploy the Ingress controller such as Traefik / Kong and configure the Ingress accordingly.


### How to proceed
1) Clone this repository on your local machine and start a new local repository.
2) Write the code.
3) Write the documentation.
4) The repository should contain the modified application and all other DevOps files and scripts in a separate folder
4) Create a repo on Github and push your code on it


## Extra Credit
* Monitoring implementation
* Database backup and restore

## Support
Feel free to contact us it-admin@tradeling.com for any questions.
