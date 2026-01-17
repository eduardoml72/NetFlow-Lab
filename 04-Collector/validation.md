# NetFlow Validation

## Validation Steps

1. Start NetFlow service on collector
2. Generate traffic from Kali to Windows
3. Observe incoming flows
4. Validate:
   - Source IP
   - Destination IP
   - Ports
   - Protocol

---

## Indicators of Success
- Flows visible in dashboard
- Flow timestamps match traffic generation
- Traffic volume increases during tests

---

## Common Issues
| Issue | Cause |
|------|-------|
Collector shows no data | Firewall not exporting flows
Partial flows | Incorrect interface selection
