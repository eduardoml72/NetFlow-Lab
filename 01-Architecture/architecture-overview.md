# NetFlow Lab – Architecture Overview

## Objective
This laboratory is designed to demonstrate how NetFlow data can be collected and analyzed in a controlled environment in order to detect suspicious network activity such as SSH and RDP brute force attempts.

The lab simulates a small enterprise network using open-source components and virtualized infrastructure.

---

## Components

### Windows 11 – Endpoint
- Acts as a target system
- Generates SSH and RDP traffic
- Represents a typical corporate workstation or server

### pfSense – Firewall / Router
- Open-source firewall
- Routes traffic between different subnets
- Exports NetFlow/IPFIX data
- Acts as the single point of network visibility

### Kali Linux – NetFlow Collector
- Receives NetFlow data from pfSense
- Runs a custom Python-based NetFlow collector
- Used for traffic analysis and detection logic

---

## Network Design Rationale

The lab uses two different subnets interconnected by pfSense.  
This design ensures that all traffic between the Windows 11 endpoint and the Kali Linux collector traverses the firewall, making it visible to NetFlow.

This approach reflects real-world enterprise environments where inter-VLAN traffic is monitored at Layer 3 for security analysis.

---

## Visibility Considerations

NetFlow provides metadata about network flows such as:
- Source and destination IP
- Source and destination ports
- Protocol
- Packet and byte counts
- Flow duration

NetFlow does NOT provide:
- Payload inspection
- Authentication results
- Usernames or passwords

Because of this, NetFlow is used as a detection and visibility tool, not as a full forensic solution.

---

## Use Cases Covered
- SSH brute force attempts (pattern-based detection)
- RDP unauthorized access attempts
- Traffic volume and frequency analysis
- SOC-style investigation workflows

---

## Limitations
- No payload inspection
- Detection is based on behavioral patterns
- Requires correlation with endpoint logs for confirmation
