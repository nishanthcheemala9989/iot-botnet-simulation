\# IoT Botnet Simulation \& Detection (CCNS)



Docker-based lab project to simulate IoT botnet-style command \& control over MQTT and observe network behavior using monitoring / IDS.



\## What this demonstrates

\- MQTT broker (Mosquitto) used as messaging backbone

\- C2 server publishes commands and receives device telemetry

\- Device simulators publish periodic telemetry

\- Victim service to validate controlled request behavior

\- Optional monitoring: Prometheus + Grafana

\- Optional IDS: Suricata / Zeek (outputs ignored in Git)



\## Architecture

Device(s) -> MQTT Broker -> C2 Server

C2 Server -> Victim Server (controlled traffic)

Monitoring: Prometheus scrapes metrics, Grafana dashboards



\## Tech Stack

\- Docker / Docker Compose

\- Python (paho-mqtt)

\- Mosquitto (MQTT)

\- Prometheus + Grafana (optional)

\- Suricata / Zeek (optional)



\## How to run

1\) Install Docker Desktop

2\) From project root:

&nbsp;  docker compose up -d --build

3\) Check containers:

&nbsp;  docker ps



\## Repo structure

\- c2/                 : C2 server code + Dockerfile

\- device/             : IoT device simulator

\- victim/             : victim service

\- mosquitto-config/   : broker config

\- monitoring/         : prometheus/grafana configs (optional)



\## Safety / Disclaimer

This is a controlled academic lab simulation. No real-world attack usage.



\## Resume bullets (copy-ready)

\- Built a multi-container IoT security lab using Docker Compose (MQTT broker, C2, device simulators, victim service).

\- Implemented MQTT telemetry + command channel and validated behavior using monitoring/IDS tooling (Prometheus/Grafana, Suricata/Zeek).



