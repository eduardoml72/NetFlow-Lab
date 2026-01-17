# NetFlow Configuration

## NetFlow Protocol
- Version: NetFlow v9 / IPFIX
- Transport: UDP
- Listening Port: 2055

---

## Collector Settings
- NetFlow receiver enabled
- Flow aggregation enabled
- Retention configured for lab usage

---

## Expected Sources
| Device | IP |
|------|----|
| pfSense | 10.0.60.1 |

---

## Security Considerations
- Collector listens only on internal interface
- No external exposure
