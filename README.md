
# DevOps WebApp Pipeline

This is a sample DevOps pipeline project featuring:

- Node.js Express web application
- Docker and Docker Compose for orchestration
- Jenkins for CI/CD
- AWS (via Terraform) - optional for S3/EKS setup
- Prometheus + Grafana for monitoring

## Run Locally

```bash
docker-compose up --build
```

Visit:
- App: http://localhost:3000
- Prometheus: http://localhost:9090
- Grafana: http://localhost:3001

## CI/CD

Jenkins pipeline is defined in `Jenkinsfile`. It builds, tests, and deploys the app using Docker Compose.

## Monitoring

Prometheus scrapes metrics from the app and Grafana visualizes them.

## Terraform (Optional)

Provision AWS infra with files in `/terraform`.

## License

MIT
