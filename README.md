# 🏠 Homelab — Raspberry Pi 400

Praktisches Homelab auf einem Raspberry Pi 400 — aufgebaut während meiner FISI-Ausbildung bei GFN GmbH Hamburg.

## 🛠️ Was läuft hier

| Service | Tool | Zweck |
|---|---|---|
| DNS / Ad-Blocker | Pi-hole | Werbung & Tracking für alle Geräte blockieren |
| Monitoring | Prometheus + Grafana | CPU, RAM, Netzwerk überwachen |
| Container | Docker | Services isoliert betreiben |


## 🗺️ Architektur

**Netzwerk:** Speedport Smart 4 (192.168.2.1)

| Gerät | IP | Rolle |
|---|---|---|
| Raspberry Pi 400 | 192.168.2.186 | Server — Pi-hole, Grafana, Docker |
| Laptop (AKPRIVAT) | 192.168.2.128 | Entwicklung & Verwaltung |
| iPhone / iPad | 192.168.2.x | Pi-hole DNS Client |
| Smart-TV / Echo | 192.168.2.x | Pi-hole DNS Client |


## 🚀 Was ich dabei gelernt habe

- Netzwerk-Scanning mit **Nmap**
- DNS-Funktionsweise und Pi-hole-Konfiguration
- Docker & Docker Compose
- Prometheus + Grafana Monitoring-Stack
- SSH-Zugriff auf Linux-Server
- Ethical Hacking Grundlagen (TryHackMe)

## 📈 Status

- ✅ Pi-hole aktiv — 84.231 Domains geblockt
- ✅ Grafana Dashboard live
- ✅ Prometheus Metriken aktiv
- 🔄 TryHackMe Lernpfad in Bearbeitung

## 🔧 Hardware

- Raspberry Pi 400 (4GB RAM)
- 16GB MicroSD
- LAN-Kabel direkt am Router
