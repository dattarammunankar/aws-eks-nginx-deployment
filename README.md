## Project Overview This project involves setting up a managed Kubernetes cluster on AWS EKS and deploying a containerized Nginx application. The application is exposed to the internet using a LoadBalancer service.

## Tech Stack

Cloud: AWS (EKS, EC2, IAM)

Orchestration: Kubernetes

Tools: eksctl, kubectl, AWS CLI

## Steps Taken

Management Server: Configured an EC2 instance with an IAM Role (AdministratorAccess) to manage the EKS lifecycle.

Cluster Provisioning: Used eksctl to create a 2-node managed cluster in us-east-1.

App Deployment: Deployed Nginx pods using kubectl.

External Access: Created a LoadBalancer service to route external traffic to the pods.

## Verification (Output)

kubectl get nodes (Nodes are in Ready state)

kubectl get svc (LoadBalancer External IP is generated)

Application URL: http://a9c09967192b3422aafd5d00de474a6e-1927301693.us-east-1.elb.amazonaws.com/
