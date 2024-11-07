# Task Details

## Objective

The objective of this task is to assess your skills in application development, containerization, Kubernetes deployment, monitoring, and automation.

---

## Task Requirements

1. **Develop a Python Application**:
   - Create a Python application that checks if `google.com` is up and running.
   - The application should expose a web interface that shows whether `google.com` is "Up" or "Down".

2. **Containerize the Application**:
   - Write a `Dockerfile` to containerize the Python application.
   - Ensure the container runs with minimal dependencies.

3. **Deploy on Kubernetes**:
   - Use the Kubernetes cluster provided by Docker Desktop.
   - Create Kubernetes manifests to deploy the containerized application:
     - **Deployment**: Define the deployment specifications for the application.
     - **Service**: Expose the application as a service within the cluster.

4. **Monitoring Setup**:
   - Configure monitoring for the application using **Prometheus** and **Grafana**.
   - Collect basic metrics like request count, response status, and latency.
   - Include Kubernetes manifests or configurations to deploy Prometheus and Grafana in the same cluster.

5. **Automation Script**:
   - Create a shell script (`deploy.sh`) that:
     - Sets up the entire environment (deploys the application and monitoring).
     - Tears down the environment (removes all resources).
   - Ensure the script is idempotent and can be run multiple times without issues.

---

## Task Instructions

1. **Application Development**:
   - Write a Python script that performs an HTTP check on `google.com`.
   - The script should return a simple HTML page saying "Google is Up" or "Google is Down" based on the HTTP response.
   - Use a lightweight web framework like Flask to handle HTTP requests.

2. **Dockerize the Application**:
   - Create a `Dockerfile` in the `docker/` folder.
   - Ensure the image is as lightweight as possible, focusing on a small footprint and efficiency.
   - Build and run the container locally to verify its functionality before proceeding.

3. **Kubernetes Deployment**:
   - Create the following Kubernetes manifests in the `k8s/` folder:
     - `deployment.yaml`: Defines the Deployment for the application.
     - `service.yaml`: Defines a Service to expose the application within the cluster.
   - Deploy these resources on Docker Desktop’s Kubernetes cluster to confirm they work as expected.

4. **Monitoring Setup**:
   - Create a `monitoring.yaml` in the `k8s/` folder.
   - This file should:
     - Set up Prometheus to scrape metrics from the application.
     - Deploy Grafana for visualizing the metrics.
   - Verify that Prometheus can collect and Grafana can display metrics like application uptime, request count, and latency.

5. **Automation Script**:
   - Create a shell script named `deploy.sh` in the `scripts/` folder.
   - The script should:
     - Deploy the application, service, and monitoring components in the Kubernetes cluster.
     - Include commands to set up and tear down the environment.
     - Be able to both start and stop the entire setup with a single command.
---