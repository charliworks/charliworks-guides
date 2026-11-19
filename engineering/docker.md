# Docker

> Last reviewed: 2026-11 · Applies to: Dockerized projects

## TL;DR (the rules)

- `docker compose up` must bring up a working local environment with no extra steps. Put any extra steps in the README.
- Pin base image versions (`node:22-alpine`, not `node:latest`).
- Use multi-stage builds so production images contain no build tooling.
- Run as a non-root user in production images.
- Use a `.dockerignore` that excludes `.env`, `node_modules`, `.git`, and tests.
- Secrets come from `env_file` or the runtime environment, never `ENV` or `COPY` in the Dockerfile.
- Use named volumes for databases, and back them up ([backups](backups.md)).
- Add a health check for each service.
- Service names in `compose.yaml` are `kebab-case` and match the README.
