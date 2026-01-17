# NetFlow Collector Overview

## Purpose
The NetFlow Collector is responsible for receiving, storing, and visualizing flow data exported by the pfSense firewall.

---

## Selected Tool
- Tool: ntopng + nProbe
- Reason:
  - Open source
  - Supports NetFlow/IPFIX
  - Web-based visualization
  - Commonly used in SOC environments

---

## Data Collected
- Source and destination IP
- Source and destination ports
- Protocol
- Byte and packet count
- Flow duration

---

## SOC Use Cases
- Detection of lateral movement
- Identification of scanning activity
- Detection of abnormal DNS traffic
