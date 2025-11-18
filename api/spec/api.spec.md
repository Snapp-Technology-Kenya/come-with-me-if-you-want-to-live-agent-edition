# API Specification

## Architecture

The API is a restful service that is split into read/write (CQRS) services. The read service queries a postgres database, and the write service puts events onto a RedPanda event stream. Both services are built using Bun. The target environment is Kubernetes.

- JSON REST API
- Bun
- Kubernetes
- PostgreSQL
- RedPanda

We assume all connection strings and secrets are provided via .env files mounted from kuberentes secrets.

## Endpoints