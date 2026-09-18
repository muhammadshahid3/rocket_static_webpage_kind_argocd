# Mission Control — Rocket Launch Site

A single-page HTML/CSS/JS site: click **LAUNCH**, watch a countdown, liftoff with
flame and smoke, ascent telemetry (altitude/velocity/stage), then the view switches
to space and the rocket settles into a looping orbit around Earth. Click **RELAUNCH**
to reset and go again.

## Run it directly (no Docker)
Just open `index.html` in any browser. Everything (HTML/CSS/JS) is in that one file.

## Run it with Docker

Build and run:
```bash
docker build -t rocket-site .
docker run -p 8080:80 rocket-site
```
Then open http://localhost:8080

Or with docker-compose:
```bash
docker compose up --build
```
Then open http://localhost:8080

## Files
- `index.html` — the entire site (markup, styles, animation logic)
- `Dockerfile` — serves `index.html` with nginx:alpine
- `docker-compose.yml` — convenience wrapper (maps port 8080 → 80)
# rocket_static_webpage_kind_argocd
