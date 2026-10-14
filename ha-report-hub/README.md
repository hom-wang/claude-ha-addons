# HA Report Hub

Serves the folder `/config/ha-report-hub/` (generated weekly by claude-ha's `ha_hub.py`) behind Home Assistant login.

- Accepts connections only from the Supervisor Ingress proxy (172.30.32.2); no port is exposed.
- Mounts `/config` read-only and never writes anything.
- No configuration options. To update, bump `version` in `config.yaml`.
