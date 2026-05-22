# Deploying Applications on AWS ECS with Docker

A step-by-step guide to deploying containerized applications on **Amazon ECS (Elastic Container Service)** using **Amazon ECR (Elastic Container Registry)** and **Docker**.

## Overview

This repository documents the process of containerizing an application with Docker, pushing the image to Amazon ECR, and deploying it to a production-ready ECS cluster — covering the full container deployment lifecycle on AWS.

## What's Covered

- **Docker** — Containerizing the application and building Docker images
- **Amazon ECR** — Pushing and managing container images in a private registry
- **Amazon ECS** — Creating task definitions, services, and clusters
- **IAM Roles** — Configuring permissions for ECS tasks to access AWS resources
- **Networking** — Setting up VPC, subnets, and security groups for ECS
- **Load Balancing** — Integrating an Application Load Balancer (ALB) with ECS services

## Architecture

```
Developer → Docker Build → ECR (Image Registry) → ECS Task Definition → ECS Service → ALB → Users
```

## Key Steps

1. **Containerize the app** — Write a `Dockerfile` and build the image
2. **Push to ECR** — Authenticate Docker to ECR and push the image
3. **Create ECS Cluster** — Set up a Fargate or EC2-backed ECS cluster
4. **Define Task** — Configure the ECS task definition with the ECR image URI
5. **Deploy Service** — Launch the ECS service and attach to a load balancer
6. **Monitor** — Use CloudWatch for container logs and metrics

## Technologies

| Technology | Purpose |
|------------|---------|
| Docker | Application containerization |
| Amazon ECR | Private container image registry |
| Amazon ECS | Container orchestration |
| AWS Fargate | Serverless compute for containers |
| Application Load Balancer | Traffic distribution |
| CloudWatch | Logging and monitoring |

## Author

**Raj Bhoge** — Cloud & AI Engineer  
[GitHub](https://github.com/RajBhoge) | [LinkedIn](https://www.linkedin.com/in/raj-bhoge-834280194/) | [Blog](https://rajbhoge2107.hashnode.dev/)
