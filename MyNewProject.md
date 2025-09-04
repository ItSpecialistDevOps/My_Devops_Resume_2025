# CI/CD with Jenkins & MyNewProject

## Objective
Automate build and deployment pipeline for a GitHub-hosted application.

## Work Done
- Cloned source code from GitHub.
- Configured Jenkins pipeline with stages:
  1. Clone repository
  2. Build Docker image
  3. Run **SonarQube** code analysis
  4. Run **Trivy** scan on built image
  5. Push image to Docker Hub
  6. Deploy on server/Kubernetes
- Integrated GitHub webhook for automatic trigger.

## Technologies Used
- Jenkins
- GitHub
- Docker
- Kubernetes
- SonarQube
- Trivy

## Repository
[GitHub Repo → MyNewProject](https://github.com/ItSpecialistDevOps/MyNewProject)
