# my-server

Simple WebSocket server, deployed via a public GitHub link.

- Start: `node server.js`
- Listens on `0.0.0.0:$PORT` (platform sets `PORT=8080`)
- WebSocket path: `/ws`
- Health: `GET /`, `GET /generate_204`, `GET /flclash.yaml`

## Required env vars

Set these in the platform dashboard, not in the repo:

- `SERVER_UUID` — your UUID, required. Do not commit a real UUID.
- `SERVER_PATH` — optional, default `/ws`
- `PORT` — set by the platform, default `3000` locally

Note: the subscription output still has to name the protocol type for the client to parse it. Variable names, env var names, and paths in this repo are neutral.
