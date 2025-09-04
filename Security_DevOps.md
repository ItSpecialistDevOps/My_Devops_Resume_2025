### 4. **Security_DevOps.md**
```markdown
# Security in DevOps (DevSecOps)

## SonarQube
- Deployed SonarQube container (`9000:9000`).
- Configured Jenkins pipeline to run **SonarQube code analysis**.
- Generated reports on code smells, bugs, and vulnerabilities.
- Improved code quality metrics before deployment.

## Trivy
- Installed and used **Trivy** for Docker image scanning.
- Scanned application images (todo, hello-nginx-container, Jenkins).
- Identified and fixed OS & dependency-level CVEs.
- Integrated scans into CI/CD pipeline for automated checks.

## Example Trivy Command
```bash
trivy image itspecialistdevops/todo-app:latest
