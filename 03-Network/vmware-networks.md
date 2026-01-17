# VMware Network Configuration

## Virtual Network Design
This lab uses VMware Workstation virtual networks to simulate segmented enterprise networks.

---

## VMware Networks Used

### VMnet8 – NAT
- Provides internet access
- Used as pfSense WAN interface
- Represents an external/untrusted network

### VMnet1 – Host-Only
- Used for internal lab communication
- No direct internet access
- Used for LAN and internal segments

---

## Network Mapping

| VM | Interface | VMware Network |
|----|----------|----------------|
| pfSense | WAN | VMnet8 |
| pfSense | LAN | VMnet1 |
| Windows 11 | NIC | VMnet1 |
| Kali Linux | NIC | VMnet1 |

---

## Rationale
Using NAT for the WAN interface allows pfSense to simulate a perimeter firewall while maintaining internet access for updates and testing.
