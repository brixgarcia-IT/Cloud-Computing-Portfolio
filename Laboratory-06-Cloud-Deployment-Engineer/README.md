# Mission 6: The Cloud Deployment Engineer

## Mission Overview

This mission demonstrates how to deploy a two-tier private cloud storage application using Docker Compose. The deployment consists of Nextcloud as the web application and MariaDB as the database.

## Objectives

- Explain two-tier application architecture.
- Create a Docker Compose YAML configuration.
- Deploy Nextcloud and MariaDB as separate containers.
- Access the Nextcloud web interface through port 8080.
- Document deployment and teardown procedures.
- Apply Infrastructure as Code (IaC) principles.

## Commands Executed

```bash
mkdir nextcloud-deployment
cd nextcloud-deployment
nano docker-compose.yml
cat docker-compose.yml
docker compose up -d
docker compose ps
docker compose logs
docker compose down
```

## Skills Learned

- Understanding multi-tier application architecture.
- Writing and editing YAML configuration files.
- Deploying multiple containers with Docker Compose.
- Configuring application and database communication.
- Accessing a containerized web application.
- Documenting technical procedures using Markdown.
- Understanding Infrastructure as Code (IaC).

## Screenshots

Deployment evidence is available in the `screenshots/` directory.

- `compose-deployment.png` — running containers.
- `nextcloud-web.png` — Nextcloud installation page.
- `compose-teardown.png` — container teardown evidence.
