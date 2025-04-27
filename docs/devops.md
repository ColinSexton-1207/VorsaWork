# DevOps Overview

## CI/CD
- GitHub Actions workflow per push to `main`:
  - Runs tests
  - Builds Docker images
  - Pushes to container registry **(later)**

## Containerization
- Each service has a `Dockerfile`
- Local orchestration via `docker-compose`
- Future: **Kubernetes deployment w/ Helm (optional)**

## Monitoring
- **Prometheus for metrics** [^1]
- **Grafana for dashboards** [^1]
- **Loki or ELK for logs** [^1]

## Secrets
- Locally: `.env` + `application.yml`
- Future: **AWS Secrets Manager or K8s secrets** [^2]

[^1]: Decisions for these tools are still currently in progress, the list may change in the future.
[^2]: Going to look into additional layers of security that may expand on these tools.