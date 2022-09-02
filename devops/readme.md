# Tradeling DevOps Challenge
<p align="left">
<a href="https://tradeling.com"><img src="https://c8n.tradeling.com/assets/svgs/tradeling-logo.svg" alt="Tradeling" width="250"/></a>
</p>

## The Goal

Your task is to setup a kubernetes cluster and deploy traefik as Ingress, REST API and a frontend that consumes the REST API into it and to have a fully automated CI/CD solution.

We prefer well-thought-out solutions over the quick-and-dirty kind. So take your time, if you need it. A rushed job is usually matched by a swift rejection.

## The Process

> Note: a free-tier account can be used to do the task.

1. Setup a kuberentes cluster using [kOps](https://kops.sigs.k8s.io/).
2. When you have a running cluster, deploy [Traefik](https://doc.traefik.io/traefik/).
3. Deploy an API of your choice and a frontend application of your choice that consumes the API into the cluster. This can be a handwritten hello world application or any other ready-made docker images.
4. Implement a CI/CD for the application using [Github Actions](https://github.com/features/actions)
5. Automate the whole infrastructure resources creation using [Terraform](https://www.terraform.io/).
6. Automate the application deployment using [Helm](https://helm.sh/).
7. Document your solution and Draw a diagram for the infrastructure and the deployed application

## Acceptance Criteria

- The code you've written to create the cluster and deploy the applications.
- Proven evidence (you can send it as screenshots) for the infrastructure and the application deployment.

## Bonus Round (not required, but nice-to-have)

- Set up logging for the cluster using datadog or any other tool. You should be able to see the individual log events with 404, 200 status codes
- Set up monitoring for the cluster and create a k8s dashboard with necessary metrics to check if the cluster is healthy
- Create slack alerts for events including but limited to  HTTP 404, 403 events when it happen (you can set a threshold and trigger the notification based on the threshold configuration)

## How we're evaluating the result

- Feature Completeness: Does your cluster fulfil all acceptance criteria?
- Code Quality: If you've written any code to achieve the task, is the code clean, well-structured and easy to understand?
- Security:
    - How secure is your setup?
    - Have you followed any best practices or standards for the Dockerfiles that you have used?
    - Have you followed any best practices or standards for deploying the infastructure on AWS and kubernetes?
- Documentation: How good is the documentation?
- The extra mile: Did you hit any bonus goals?
