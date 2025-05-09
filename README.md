# SOC-LAB-Blue-Team-Red-Team
A full enterprise-ready detection lab using Virtualbox VMs to simulate network attacks and monitor them with Suricata IDS and Splunk.
This lab was built to simulate real-world SOC workflows, using Suricata as the IDS and Splunk for centralized log aggregation and visualization. 
Blue Teamers, defenders, and aspiring SOC analysts



## 🛡️ Incident Detection Report – Brute Force

**Date:** April 20th, 2025 - May 4th, 2025  
**Analyst:** Grisham D.  
**Detection System:** Suricata + Splunk  
**Attack Type:** Brute Force (RDP)  
**Attacker IP:** 192.168.50.255 (Kali)  
**Target IP:** 192.168.50.10 (Windows 10 Server)

---

## 🔍 Summary

Simulated a brute force attack using Hydra. Detected via Suricata and logged to Splunk. Confirmed presence of:
- Suricata alert: `ET ATTACK Brute Force`
- Event timestamps, source port, and target IP
- Log entry: `event_type: alert`, `proto: tcp`, `dest_port: 3389`

---

## 📸 Screenshots
- Suricata alert in eve.json
- Splunk dashboard or log view


<br/>

## Environment Setup
- Ubuntu Server - ifconfig
<img src="https://i.imgur.com/XQiUihb.png">
- Ubuntu Server - ip a
<img src="https://i.imgur.com/UkBtRCQ.png">
- Windows 10 Server
<img src="https://i.imgur.com/FSYYEGC.png">
- Windows 10 Workstation
<img src="https://i.imgur.com/FSYYEGC.png">
- Kali Linux Attacker Machine - ipconfig
<img src="https://i.imgur.com/fN4WjEL.png">
- Kali Linux Attacker Machine - ip a 
<img src="https://i.imgur.com/fN4WjEL.png">
  
- Attack Simulation

- Hydra Bruteforce RDP
<img src="https://i.imgur.com/FcFwAHV.png">
- Nmap Port Scan on Windows 10 Server
<img src="https://i.imgur.com/5sWO6W8.png">

  
- Suricata
<img src="https://i.imgur.com/tsSikfa.png">

- Splunk Ingestion & Visualization
<img src="https://i.imgur.com/UVYlYas.png">

- Suricata Detection
<img src="https://i.imgur.com/pwK9aWY.png">
  
  
<br />

