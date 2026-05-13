# AdGuard Home Stack

Network-wide DNS ad blocker running on the DS920+ Synology NAS at `192.168.1.90`.

Web UI: `http://192.168.1.90:8080`

## Ports

| Port | Protocol | Purpose |
|---|---|---|
| 53 | TCP/UDP | DNS |
| 3000 | TCP | Initial setup wizard (first run only) |
| 8080 | TCP | Web UI |

## Environment Variables

| Variable | Description |
|---|---|
| `ROOT_PATH` | Base path for config/data on the NAS (e.g. `/volume1/docker`) |

## First-time Setup

1. Deploy the stack via Komodo
2. Visit `http://192.168.1.90:3000` to complete the setup wizard
3. Set the web interface port to `80` during setup
4. Point your router's primary DNS to `192.168.1.90`

## Updating

Redeploy via Komodo to pull the latest image.
