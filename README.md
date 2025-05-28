# AWS ECS + EC2 - CLOUDFORMATION

This repository contains YAML configuration files for deploying services on AWS using CloudFormation.

## 🚀 Description

This project facilitates the deployment of infrastructure on AWS using ECS ​​with EC2 instances. Here you will find the files needed to automatically create and manage resources on AWS.
This deployment includes an application developed in FastAPI, packaged in a Docker image, and hosted on AWS ECR.

## 📂 Repository Structure
* Cluster-Deploy.yml: Defines the ECS cluster based on EC2 instances, Autoscaling...
* VPC.yml: Configures the VPC, subnets, routes...
* Service.yml: Creates **ListenerRuleHealthCheck**, **TaskDefinition**, **ECSService**...
* ELB.yml: Defines the **ALB**, **Security Group**, and **Listener** configuration...

## 📌 Requirements

Before deploying these files, make sure you have:

- An **AWS** account with permissions to use CloudFormation, ECS, and EC2.
- **AWS CLI** installed and configured with valid credentials.
- **Docker** installed to build the application image.
- **FastAPI** installed if you want to test the application locally before deploying.

### 📌 Notes

- Parameters such as service names, subnets, and role ARNs should be adjusted according to your environment.
- Review file dependencies before deploying.
- You can modify the YAML definitions according to your project's requirements.
- Make sure to update the image in ECR before updating the stack.

📌 **Author:** [charleetrion](https://github.com/charleetrion)
🛠️ **Technologies:** AWS CloudFormation, ECS, EC2, Secrets Manager, Load Balancer, FastAPI, Docker
