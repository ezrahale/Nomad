# Nomad

# NOMAD v1 — Field Agent

> A portable, secure, and modular reconnaissance & analysis toolkit for low-profile digital operations. Designed for signal awareness, system profiling, and offline intelligence gathering.

---

## 🌐 Project Description

**NOMAD** is a lightweight, tactical field node built on Raspberry Pi Zero or similar ARM devices. It is designed for:

- Passive signal intelligence (Wi-Fi, BLE, GPS)
- LAN recon & device mapping
- Trap mode (honeypot ops)
- Session logging & report generation
- Secure emergency wipe
- Offline use, air-gapped ready

All sessions are timestamped, structured, and locally stored — no cloud, no dependencies.

---

##  Modes & Tools

### 1.Recon Mode
- Maps local subnet, devices, and ports
- Captures nearby Wi-Fi networks
- Scans BLE and GPS (if enabled)
- Auto-labels MACs by vendor
- Stores full session logs and summaries

### 2.Signal Analyzer
- Wi-Fi signal snapshot
- BLE beacon scanner
- Signal strength monitoring over time
- Interface health and RF state
- Combines into one `signal_report.txt`

### 3.Trap Mode (Coming)
- Fake AP or honeypot mode
- Device attraction + behavior logging

### 4.Device Profiler
- Gathers internal hardware + OS stats
- CPU, memory, uptime, MACs, open ports
  
### 5.Session Summary
- Browse past session logs easily

### 6.Emergency Wipe
- Securely delete all ops & logs

---

## Data Structure

All logs are saved in organized folders:

```bash
data/
├── sessions/         # Recon sessions
├── signal_logs/      # Signal Analyzer logs
├── gps/              # GPS NMEA or parsed
├── vault/            # Sensitive exports
