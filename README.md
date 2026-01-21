# IoT Botnet Simulation (CCNS Project)

Docker-based lab simulation of IoT botnet behavior using MQTT (Mosquitto) with:
- C2 server
- Device simulators (telemetry)
- Victim HTTP server
- Optional monitoring (Prometheus/Grafana)
- Optional IDS outputs (Suricata/Zeek) - not committed

## How to run
1) Install Docker Desktop
2) In project folder:
   docker compose up -d --build

## Notes
This is a safe lab setup for academic demonstration.
