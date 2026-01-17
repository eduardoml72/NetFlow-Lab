# Kali Linux – NetFlow Collector and Analysis System

## Role in the Lab
Kali Linux serves as the NetFlow collector and analysis platform.  
It receives flow data exported by pfSense and processes it using a custom Python-based collector.

---

## Key Responsibilities
- Receive NetFlow data
- Parse and store flow records
- Support basic detection logic

---

## Tools Used
- Python 3
- Custom NetFlow collector script
- Command-line analysis tools

---

## SOC Relevance
This system simulates a lightweight flow collector or SIEM ingestion point commonly used in SOC environments.

---

## Notes
The collector does not actively query pfSense; all NetFlow data is sent unidirectionally from the firewall.
