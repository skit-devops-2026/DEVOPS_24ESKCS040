# Project ELARA

[![CI](https://github.com/skit-devops-2026/DEVOPS_24ESKCS040/actions/workflows/ci.yml/badge.svg)](https://github.com/skit-devops-2026/DEVOPS_24ESKCS040/actions/workflows/ci.yml)

Project ELARA is a full-stack web application with separate User and Admin applications, backend API services, and automated CI/CD pipelines.

## Author

| Roll No | Name | GitHub Username |
|---|---|---|
| 24ESKCS040 | Aman Mehta | aman-mehta99 |

## Project Structure

- User/ — User frontend application (Vite + React)
- admin/ — Admin dashboard application (Vite + React)
- backend/ — Express backend REST API service
- tests/ — Automated test suite
- .github/workflows/ci.yml — GitHub Actions CI pipeline
- Jenkinsfile — Declarative Jenkins CI/CD pipeline
- Makefile — Project automation commands
- scripts/ — Repository and hygiene checks
- docs/ — Project documentation
- monitoring/ — Monitoring configuration
- k8s/ — Kubernetes deployment manifests

## DevOps

The project uses GitHub Actions for continuous integration and automated testing.

The CI pipeline performs:
- Repository hygiene checks
- Dependency installation
- Automated tests
- User application build
- Admin application build

Jenkins is configured for automated build and deployment via `Jenkinsfile`.

## Automated Testing & Commands

```bash
# Install dependencies
make install

# Run automated tests
make test

# Build User and Admin applications
make build
```

## Health Endpoint

`GET /health` returns the running commit SHA and system status.

## Repository

https://github.com/skit-devops-2026/DEVOPS_24ESKCS040
