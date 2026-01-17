# IP Addressing Plan

## Subnets

### Subnet A – Endpoint Network
- Network: 10.0.60.0/24
- Gateway: 10.0.60.1
- Purpose: Endpoint traffic (SSH / RDP)

### Subnet B – Monitoring Network
- Network: 10.0.70.0/24
- Gateway: 10.0.70.1
- Purpose: Monitoring and NetFlow collection

---

## Host Addressing

| System | IP Address |
|------|-----------|
| pfSense (LAN) | 10.0.60.1 |
| pfSense (OPT1) | 10.0.70.1 |
| Windows 11 | 10.0.60.20 |
| Kali Linux | 10.0.70.10 |

---

## Addressing Considerations
Static IP addressing is used to ensure consistent flow visibility and simplify analysis.
