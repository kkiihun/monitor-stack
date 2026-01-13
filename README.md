# Home Monitoring Stack (Uptime Kuma + Dozzle)

Self-hosted monitoring stack running on Docker (LAN).

## Services
- Uptime Kuma: uptime checks + notifications
- Dozzle: Docker container log viewer

## Ports
- Uptime Kuma: http://<UB02_IP>:3001
- Dozzle: http://<UB02_IP>:9999

## Run
~bash
docker compose -f compose.yml up -d
docker compose -f compose.yml ps
~

## Stop
~bash
docker compose -f compose.yml down
~

## Notes
- Recommend DHCP reservation (router) so the server IP stays stable.
- Do not expose these ports to the public internet without auth + TLS.
