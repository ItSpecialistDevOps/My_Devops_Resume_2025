# Docker – Detailed Expertise

## Skills
- Created custom Dockerfiles for Node.js, Angular, and Python applications.
- Built optimized images using multi-stage builds.
- Worked with Docker Compose for orchestrating multi-container applications.
- Pushed and pulled images from Docker Hub.
- Performed container vulnerability scans with **Trivy**.
- Debugged containers with `docker exec` and logs.

## Example Dockerfile
```dockerfile
FROM node:18-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install --production
COPY . .
CMD ["node", "server.js"]
