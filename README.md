# K8s Cluster Autoscaler with AWS Auto Scaling Groups

## Overview
Implemented Kubernetes Cluster Autoscaler integrated with AWS Auto Scaling Groups to automatically scale worker nodes based on workload demand.

## Tech Stack
- Kubernetes
- AWS Auto Scaling Groups
- Node.js
- Express.js
- Docker
- k6

## Features
- Automatic node scaling
- Dynamic EC2 provisioning
- Containerized Express API
- Load testing with k6
- Cost optimization

## Project Summary
Built and deployed a Kubernetes Cluster Autoscaler solution integrated with AWS Auto Scaling Groups to dynamically scale worker nodes based on pod demand. Developed and containerized a Node.js Express API and used k6 load testing to trigger automatic cluster scaling.
## Architecture

k6 Load Generator
        |
        v
Node.js Express API
        |
        v
Kubernetes Cluster
        |
        v
Cluster Autoscaler
        |
        v
AWS Auto Scaling Group
        |
        v
EC2 Worker Nodes

## Workflow

1. Deploy Node.js application to Kubernetes.
2. Configure AWS Auto Scaling Group.
3. Install Kubernetes Cluster Autoscaler.
4. Generate traffic using k6.
5. Pending pods trigger node scale-out.
6. New EC2 instances join the cluster.
7. Traffic decreases and unused nodes scale in.

## Skills Demonstrated

- Kubernetes
- AWS
- Docker
- Node.js
- DevOps
- Autoscaling
- Load Testing
## Architecture

```text
k6 Load Generator
        |
        v
Node.js Express API
        |
        v
Kubernetes Pods
        |
        v
Cluster Autoscaler
        |
        v
AWS Auto Scaling Group
        |
        v
EC2 Worker Nodes
