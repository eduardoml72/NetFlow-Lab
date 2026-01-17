# SSH Brute Force Simulation

## Objective
Generate repeated SSH connections to observe NetFlow behavior.

## Attacker
- Kali Linux

## Target
- Linux host / pfSense

## Protocol
- TCP 22

## Tool
- Hydra

## Command
```bash
hydra -l testuser -P passwords.txt ssh://10.0.60.20
