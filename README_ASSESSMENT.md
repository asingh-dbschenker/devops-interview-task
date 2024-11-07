# Assessment Criteria

The following criteria will be used to evaluate the submission:

---

## 1. Application Functionality (20%)

- The Python application accurately checks if `google.com` is up or down.
- The application displays the correct status message ("Google is Up" or "Google is Down") on a web interface.
- The web interface is accessible and user-friendly.

---

## 2. Containerization (20%)

- The Dockerfile is optimized for a lightweight, efficient container.
- The application runs smoothly inside the Docker container.
- Adheres to best practices for Docker image creation (e.g., small image size, efficient layers).

---

## 3. Kubernetes Deployment (20%)

- The Kubernetes manifests (Deployment and Service) are correctly configured and deploy the application successfully.
- The application is accessible within the Kubernetes cluster.
- Manifests follow best practices (e.g., resource limits, proper labels, and annotations).

---

## 4. Monitoring Setup (20%)

- Prometheus is configured to scrape metrics from the application.
- Grafana dashboards are set up to visualize key metrics (e.g., uptime, request count, and latency).
- Monitoring setup is clear and functional within the Kubernetes cluster.

---

## 5. Automation Script (15%)

- The `deploy.sh` script correctly automates the setup and teardown of the application and monitoring.
- The script is idempotent and can be run multiple times without errors.
- Script handles potential errors gracefully and includes helpful output messages.

---

## 6. Documentation and Repository Structure (5%)

- The repository follows the specified structure.
- Documentation is clear, organized, and helpful for understanding and running the project.
- Additional README files (main README, task instructions, assessment criteria) are provided and properly formatted.

---

## Bonus Points (Optional)

- **Code Quality**: Clean, readable, and modular code.
- **Security**: Follows security best practices (e.g., sensitive information is not hardcoded).
- **Additional Features**: Any extra functionality added beyond the base requirements.
- **Bug Bounty**: There are some deliberate mistakes made in the instructions for this task. Find them.

---

## Scoring

- A total of **100%** can be achieved based on the above criteria.
- Bonus points may be awarded for exceptional work or additional features.

---

## Feedback

Feedback will be provided based on the above criteria, highlighting strengths and areas for improvement.

---

Thank you for your effort and good luck with the task!