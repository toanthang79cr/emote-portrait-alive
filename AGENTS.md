# AGENTS.md

## Project Overview
Static academic project page (EMO: Emote Portrait Alive). Pure HTML/CSS/JS — no build step, no backend, no external service dependencies.

## Structure
- `index.html` — main page
- `static/css/` — stylesheets (Bulma framework, Font Awesome, custom)
- `static/js/` — JavaScript (Bulma carousel/slider, Font Awesome, custom)
- `content/images/` — framework diagrams
- `content/video/` — demo videos (large MP4 files)

## Running
```bash
docker compose -f docker-compose.base44.yml up -d
```
Served by nginx on port 3000. Edits to HTML/CSS/JS files are immediately visible on page refresh — no rebuild needed.

## Verification
- `curl http://localhost:3000/` returns the HTML page
- Page loads with videos, images, and styled content
