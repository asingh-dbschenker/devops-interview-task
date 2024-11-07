# DevOps Interview Task

This repository contains a DevOps interview task designed to assess skills in application development, containerization, Kubernetes deployment, monitoring, and automation.

---

## Overview

The task requires you to:
- **Develop a Python application** that checks if `google.com` is up and displays the status on a web interface.
- **Containerize** the application using Docker.
- **Deploy** the containerized application on a Kubernetes cluster (using Docker Desktop’s Kubernetes environment or minikube).
- **Set up monitoring** for the application using Prometheus and Grafana.
- **Automate the setup and teardown** with a single shell script.

For **detailed task instructions**, please refer to the [README_TASK.md](README_TASK.md) file.

## Repository Structure

Organize your repository as follows:

```plaintext
├── docker/
│   ├── Dockerfile                   # Dockerfile for the Python app
├── k8s/
│   ├── deployment.yaml              # Kubernetes Deployment manifest
│   ├── service.yaml                 # Kubernetes Service manifest
│   ├── monitoring.yaml              # Monitoring setup for Prometheus/Grafana
├── scripts/
│   ├── deploy.sh                    # Shell script to automate setup and teardown
├── docs/
│   ├── README_TASK.md               # Detailed task instructions
│   ├── README_ASSESSMENT.md         # Assessment criteria
├── README.md                        # Main README with overview and submission instructions
```

## Submission Instructions

- Create a new GitHub repository with the above structure.
- Implement the task as outlined in docs/README_TASK.md.
- Ensure the automated script works on any machine with Docker Desktop and Kubernetes enabled.
- Submit the GitHub repository link once complete.

## Additional Notes

- The assessment criteria are available in README_ASSESSMENT.md.
- Follow best practices for Docker, Kubernetes, and shell scripting.
- Document any assumptions or additional notes in the main README or relevant README files in each directory.

Good luck!