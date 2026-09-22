# 🌟 Bright Star — Run Memory

<!-- BRIGHT_STAR_DATA — generated; do not edit -->
```json
{
  "version": 1,
  "generatedAt": "2026-09-22T14:26:28.039Z",
  "techStack": {
    "languages": [
      "Go"
    ],
    "frameworks": [
      "Gorilla Mux"
    ],
    "databases": []
  },
  "startup": {
    "command": "docker compose up -d --build",
    "port": 8080,
    "prerequisites": [],
    "envVars": {},
    "healthCheckPath": "/healthcheck"
  },
  "setup": {
    "completed": false
  },
  "auth": {
    "hasAuth": true,
    "authObjectId": "dsT15CMMPNJdEPLmkutNwk",
    "protectedResource": {
      "method": "GET",
      "url": "/settings"
    }
  },
  "hints": {
    "startup": [
      "Miniflux repo (Go, gorilla mux) has no compose file; needs Postgres. Built docker-compose.yml at repo root with services: db (postgres:15-alpine, healthcheck pg_isready) and miniflux (build from packaging/docker/alpine/Dockerfile, env DATABASE_URL=postgres://miniflux:miniflux@db/miniflux?sslmode=disable, RUN_MIGRATIONS=1, CREATE_ADMIN=1, ADMIN_USERNAME=admin, ADMIN_PASSWORD=SuperSecret123!, LISTEN_ADDR=0.0.0.0:8080), published on host port 8080. Health endpoint: GET /healthcheck returns 200 \"OK\". Start with `docker compose up -d --build`; teardown `docker compose down`."
    ]
  }
}
```
<!-- BRIGHT_STAR_DATA -->
