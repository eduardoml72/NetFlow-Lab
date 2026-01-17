# Windows 11 – Endpoint System

## Role in the Lab
Windows 11 represents a corporate endpoint or server targeted by simulated SSH and RDP access attempts.

---

## Key Responsibilities
- Generates SSH and RDP traffic
- Acts as a target for brute force simulations
- Provides endpoint-level logs for correlation

---

## Services Used
- OpenSSH Server
- Remote Desktop Protocol (RDP)

---

## Security Perspective
From a SOC perspective, this system represents a monitored asset whose network behavior is observed via NetFlow rather than deep packet inspection.

---

## Notes
Authentication success or failure is not visible in NetFlow and must be confirmed through Windows event logs.
