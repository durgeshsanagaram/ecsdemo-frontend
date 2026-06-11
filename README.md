![Build Status](https://codebuild.us-east-2.amazonaws.com/badges?uuid=eyJlbmNyeXB0ZWREYXRhIjoiMnZsWms5clp6NEwvRnJXYUsyWjBmcnBiUWVRaFVsRlpENmg3MWU0M2oxVFpEdDdtSDRVRXJJZm1NNXdGQWIrWVU5UTFHd1RZUTdnU29SV0JyeVNHU1R3PSIsIml2UGFyYW1ldGVyU3BlYyI6InVpTTNLMlRtUEV6ZzJCZ2oiLCJtYXRlcmlhbFNldFNlcmlhbCI6MX0%3D&branch=master)

## Overview

**ecsdemo-frontend** is a containerized Ruby on Rails web application designed to act as the public-facing frontend in a microservices architecture. It is primarily utilized as part of AWS container workshops to demonstrate how traffic is received and routed to backend microservices (like `ecsdemo-nodejs` or `ecsdemo-crystal`) within an Amazon ECS (Elastic Container Service) or EKS (Elastic Kubernetes Service) cluster.

### Key Features & Infrastructure Integration

* **Microservice Architecture:** Acts as the entry point for user traffic, dynamically interacting with backend services to visualize cluster routing.
* **Multi-Orchestration Support:** Includes configuration templates for various deployment workflows, including Kubernetes manifests (`/kubernetes`), AWS ECS Parameters (`ecs-params.yml`), and Mu (`mu.yml`).
* **Container-Ready:** Equipt with a `Dockerfile`, `.dockerignore`, and `docker-compose.yml` for seamless local testing and multi-container orchestration.
* **CI/CD Integration:** Contains AWS CodeBuild specification files (`buildspec.yml`, `buildspec-dockerhub.yml`) to streamline automated build and deployment pipelines.
* **Tech Stack:** Built on Ruby (58.2%) and HTML/CSS/JavaScript to deliver a lightweight, responsive dashboard tracking container metrics.

### Project Structure

* `/app` - Core MVC architecture (controllers, views, and logic for the frontend dashboard).
* `/kubernetes` - Service and deployment manifests for running on Kubernetes/EKS.
* `Dockerfile` - Docker blueprint for containerizing the Rails environment.
* `ecs-params.yml` - Configuration file supporting deployments via the `ecs-cli`.
* `docker-compose.yml` - Local multi-container environment setup.

# Amazon Containers Workshop

This is part of an Amazon Containers workshop at https://ecsworkshop.com or https://eksworkshop.com
