# NetFlow SOC Lab

This project demonstrates how **NetFlow telemetry** can be used to detect
SSH and RDP attacks in a controlled virtual SOC environment.

The lab focuses on understanding **network-based visibility**, showing what
can (and cannot) be detected using flow data, without relying on application
logs.

---

## 🎯 Objectives

- Understand how NetFlow works in real network scenarios
- Generate malicious traffic (SSH and RDP abuse)
- Observe and analyze NetFlow records
- Identify attack patterns using flow-based indicators
- Document detections from a SOC analyst perspective

---

## 🏗️ Lab Architecture

The lab is deployed using **VMware Workstation** and consists of:

- **pfSense** – Open-source firewall and NetFlow exporter
- **NetFlow Collector** – Receives and visualizes flow data
- **Kali Linux** – Attacker machine
- **Windows 11** – Victim machine

All systems run in an isolated virtual environment.

---

## 🧰 Technologies Used

- VMware Workstation
- pfSense (NetFlow exporter)
- NetFlow / IPFIX
- Kali Linux
- Windows 11
- Open-source NetFlow collector
- Git & GitHub for documentation

---

## 📁 Project Structure

