# Real-Time Seismic Data Processing and Monitoring at CWA
# Current Status and Future Directions

- Date: 2025-05-29  |  Conference: JPGU
- Authors: Da-Yi Chen, Guan-Yi Song, Yu-Hsuan Chang
- Organization: Seismological Center, CWA, Taiwan

---

## Seismic Monitoring Infrastructure

- About 60 staff at Seismological Center, ~10 on 24/7 monitoring duty
- **632 real-time stations** across Taiwan
- Three-layer architecture: Field Stations -> Integration -> Application

### Open-Source Software
| Software | Description |
|----------|-------------|
| **Earthworm** | USGS-developed, modular, real-time seismic data processing |
| **SeisComP** | Modern open-source platform, acquisition to alerts |

---

## Earthquake Early Warning (eBEAR) System

- Earthworm Based Earthquake Alert Reporting system
- Available on Docker Hub: docker pull cwadayi/earthworm_ubuntu22.04_eew:v1

### Case: 2025/01/21 M6.4 Dapu Earthquake
- EEW system successfully detected and issued alert

### Case: 2024/04/03 M7.2 Hualien Earthquake
- First and second EEW alerts with real-time intensity observations

---

## Real-Time Monitoring via Grafana

Dashboards for:
1. Wave height (OBS pressure gauge network)
2. Data latency monitoring
3. Data availability
4. EEW dissemination status
5. Seismic waveform display

---

## LLM for EEW

- Training large language models using historical seismic data

---

## Summary
1. Robust 24/7 seismic infrastructure
2. Real-time processing with Earthworm + SeisComP
3. Advanced observability via Grafana dashboards
