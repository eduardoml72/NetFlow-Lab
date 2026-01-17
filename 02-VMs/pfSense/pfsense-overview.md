# pfSense – Firewall and NetFlow Exporter

## Role in the Lab
pfSense acts as the central firewall and routing device in the lab.  
All inter-subnet traffic must traverse pfSense, making it the primary visibility point for NetFlow data.

---

## Key Responsibilities
- Layer 3 routing between subnets
- Firewall policy enforcement
- NetFlow/IPFIX export
- Traffic centralization for monitoring

---

## Why pfSense
pfSense is an open-source firewall widely used in enterprise and lab environments.  
It provides robust routing, filtering, and flow export capabilities suitable for SOC use cases.

---

## Expected Traffic
- SSH traffic (TCP/22)
- RDP traffic (TCP/3389)
- NetFlow/IPFIX exports (UDP/2055)

---

## Notes
pfSense does not inspect payloads when exporting NetFlow data.  
It provides metadata-only visibility for network flows.
