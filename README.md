# DevOps Status Dashboard

A Python Flask web application deployed on AWS EC2 using Docker and an automated Jenkins CI/CD pipeline, with Prometheus and Grafana for infrastructure monitoring.

## Overview

The DevOps Status Dashboard demonstrates a basic DevOps workflow, from source code management and automated builds to application deployment and infrastructure monitoring.

## Technologies Used

- **AWS EC2** – Application hosting
- **Linux (Ubuntu)** – Server environment
- **Python (Flask)** – Web application
- **Git & GitHub** – Version control and source code management
- **Jenkins** – CI/CD automation
- **Docker** – Application containerization
- **Prometheus** – Metrics collection
- **Node Exporter** – Linux system metrics
- **Grafana** – Monitoring dashboards

## Architecture

1. Application code is maintained in GitHub.
2. Jenkins retrieves the source code and builds the Docker image.
3. The application is deployed to an AWS EC2 instance.
4. Prometheus collects infrastructure metrics.
5. Grafana visualizes the collected metrics through dashboards.

## Features

- Flask-based web application
- Application health-check endpoint (`/health`)
- Docker-based application deployment
- Jenkins CI/CD pipeline integrated with GitHub
- Automated deployment to AWS EC2
- Infrastructure monitoring with Prometheus and Node Exporter
- Grafana dashboards for system metrics visualization

## Application Endpoints

| Endpoint | Description |
|---|---|
| `/` | Displays the dashboard |
| `/health` | Returns application health status in JSON format |

Example health-check response:

```json
{
  "status": "healthy",
  "application": "DevOps Status Dashboard",
  "version": "1.0"
}
```

## Monitoring

Prometheus and Grafana are used to monitor infrastructure performance.

The monitoring setup can visualize metrics such as:

- CPU utilization
- Memory utilization
- Disk utilization
- Network activity

Metric availability depends on the exporters and Prometheus scrape configuration.

## Deployment Workflow

1. Push application changes to GitHub.
2. Jenkins checks out the latest source code.
3. Jenkins builds the Docker image.
4. The pipeline deploys the application to the configured EC2 instance.
5. Verify the application and health-check endpoint.
6. View infrastructure metrics in Grafana.

## Project Structure

```text
devops-status-dashboard/
├── app/
│   ├── app.py
│   ├── templates/
│   └── requirements.txt
├── Dockerfile
├── docker-compose.yml
├── Jenkinsfile
└── README.md
```

*Adjust the structure above to match your actual repository files.*

## What I Learned

- Building and containerizing a Python web application
- Creating a Jenkins CI/CD pipeline
- Deploying applications on AWS EC2
- Managing Docker containers in a Linux environment
- Collecting infrastructure metrics with Prometheus
- Creating monitoring dashboards with Grafana
- Troubleshooting deployment and monitoring issues

## Author

**Vaishnavi Swami**

GitHub: [@vaishnaviswami410](https://github.com/vaishnaviswami410)
