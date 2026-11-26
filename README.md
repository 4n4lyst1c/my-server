# my-server

Simple WebSocket server, deployed via a public GitHub link.

- Start: `node server.js`
- Listens on `0.0.0.0:$PORT` (platform sets `PORT=8080`)
- WebSocket path: `/vless`
- Health: `GET /`, `GET /generate_204`, `GET /flclash.yaml`

## Required env vars

Set these in the platform dashboard, not in the repo:

- `VLESS_UUID` — your UUID, required. Do not commit a real UUID.
- `VLESS_PATH` — optional, default `/vless`
- `PORT` — set by the platform, default `3000` locally
