# Project 1 — Containerized Web App Deployment

## Real-world problem
A small business needs a reliable way to package and deploy an internal service consistently across developer laptops and a cloud VM.

## What this project demonstrates
- Docker containerization
- Linux/container networking
- Environment configuration
- Health checks
- GitHub Actions CI/CD
- Cloud VM deployment prototype

## Architecture
Developer -> GitHub -> GitHub Actions -> Docker image -> Cloud VM -> Web app

## Local run
```bash
docker compose up --build
```
Open http://localhost:8000

## Cloud deployment
The workflow is intentionally template-based. Add repository secrets:
- VM_HOST
- VM_USER
- VM_SSH_KEY

Then configure the VM with Docker and Git.

> Security note: never commit real credentials or private keys.

## Portfolio impact
This is the foundation project. It shows that you understand how an application moves from source code to a repeatable containerized deployment.
