# Routing Design

## Routing Strategy
pfSense acts as the Layer 3 routing device between the endpoint and monitoring networks.

All traffic between different subnets must traverse pfSense, ensuring full NetFlow visibility.

---

## Traffic Flow Example

1. Kali initiates SSH connection to Windows 11
2. Traffic reaches pfSense (gateway)
3. pfSense routes traffic to destination subnet
4. NetFlow data is generated and exported

---

## SOC Perspective
Routing through a central firewall allows analysts to observe lateral movement and remote access patterns at the network layer.
