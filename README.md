# SecureFlow CI
## Secure DevSecOps CI/CD Pipeline using GitHub Actions

## Project Overview

This project demonstrates an **end-to-end DevSecOps CI/CD pipeline** built using GitHub Actions.
It automates code validation, security scanning, containerization, and deployment for a simple Python web application.

The pipeline integrates **code quality checks, security scans, Docker image creation, and automated deployment workflows**.

This project showcases how modern DevSecOps practices can be implemented using GitHub-native tools.

---

## Application Stack

* Python (Flask application)
* HTML frontend
* Docker containerization

Application files:

* `app.py` – Python web application
* `index.html` – frontend page
* `requirements.txt` – Python dependencies
* `Dockerfile` – container build configuration

---

## DevSecOps Pipeline Architecture

The CI/CD pipeline is implemented using **GitHub Actions workflows**.

Pipeline stages include:

1. Code Quality Checks
2. Linting
3. Dependency Scanning
4. Secret Detection
5. Container Image Build
6. Image Security Scanning
7. Deployment

Each stage is implemented using separate **YAML workflow files**.

---

## GitHub Actions Workflows

| Workflow               | Purpose                                      |
| ---------------------- | -------------------------------------------- |
| CICD.yml               | Main CI/CD workflow                          |
| code-quality.yml       | Static code quality checks                   |
| docker-lint.yml        | Dockerfile linting                           |
| dependency-scan.yml    | Dependency vulnerability scanning            |
| secrets-scan.yml       | Secret detection using GitLeaks              |
| image-scan.yml         | Container vulnerability scanning using Trivy |
| docker-build-push.yml  | Build and push Docker image                  |
| deploy-server.yml      | Deploy application to server                 |
| devsecops-pipeline.yml | Complete DevSecOps workflow                  |

---

## Security Integrations

The pipeline integrates **DevSecOps practices** including:

* Dependency vulnerability scanning
* Container image scanning
* Secret detection
* Code quality validation

Tools used:

* Trivy
* GitLeaks
* Docker
* GitHub Actions

---

## Containerization

The application is containerized using Docker.

Steps:

1. Build Docker image
2. Run container locally
3. Push image through pipeline
4. Deploy containerized application

---

## Project Structure

```
.github/workflows
   CICD.yml
   code-quality.yml
   dependency-scan.yml
   image-scan.yml
   secrets-scan.yml
   docker-build-push.yml
   deploy-server.yml
   docker-lint.yml

app.py
index.html
Dockerfile
docker-compose.yml
requirements.txt
README.md
```

---

## Key DevOps Concepts Demonstrated

* CI/CD pipeline automation
* DevSecOps integration
* Infrastructure automation using YAML workflows
* Containerized application deployment
* Security scanning in pipelines
* GitHub Actions workflow orchestration

---

## Author

Pramod Tidke
DevOps Engineer | Cloud & Automation Enthusiast
