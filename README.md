# Docker Checklist API

A minimal Node.js HTTP API, containerized with Docker.

## Requirements
- Docker Engine / Docker Desktop installed

## Build and run (Docker only)
```bash
docker build -t checklist-api .
docker run -p 3000:3000 checklist-api
```

## Build and run (Docker Compose)
```bash
docker compose up --build
```
Stop it with:
```bash
docker compose down
```

## Endpoints
- `GET /` → returns JSON including student ID
- `GET /health` → returns `{"status":"ok"}`

## Port
The API listens on port **3000** (mapped to host port 3000).

## Test
```bash
curl http://localhost:3000/
curl http://localhost:3000/health
```
