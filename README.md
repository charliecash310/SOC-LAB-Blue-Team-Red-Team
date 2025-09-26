# SOC-LAB-Blue-Team-Red-Team
A full enterprise-ready detection lab using Virtualbox VMs to simulate network attacks and monitor them with Suricata IDS and Splunk.
This lab was built to simulate real-world SOC workflows, using Suricata as the IDS and Splunk for centralized log aggregation and visualization. 
Blue Teamers, defenders, and aspiring SOC analysts



## 🛡️ Incident Detection Report – Brute Force

**Date:** April 18th, 2025 - May 4th, 2025  
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
## VM Adapter Settings
- Adapter 1 - NAT Network // Corporate Network
<img src="https://i.imgur.com/nlheQDn.png">

- Adapter 2 - Lab Network - labnet
<img src="https://i.imgur.com/oJAYLxO.png">

- Adapter 3 - NAT
<img src="https://i.imgur.com/lxGOfgQ.png">

- Ubuntu Server - ifconfig
<img width="652" height="648" alt="Ubuntu_Server_Network_Settings" src="https://github.com/user-attachments/assets/b2b003d4-b4a1-4f12-9c08-c3137819f3bd" />

- Ubuntu Server - ip a
<img width="806" height="457" alt="Ubuntu_Server_Network_Settings_ipa" src="https://github.com/user-attachments/assets/961995d8-7e5d-4deb-bc98-9244575b3531" />

- Windows 10 Server
<img width="730" height="740" alt="Windows_10_Workstation_Network_Settings" src="https://github.com/user-attachments/assets/413ba8f3-2a5e-491d-a916-cf3e4d695df1" />

- Windows 10 Workstation
<img src="https://i.imgur.com/y1VEAGz.png">

- Kali Linux Attacker Machine - ipconfig
<img width="671" height="618" alt="Kali_Attacker_Machine_Network_Settings" src="https://github.com/user-attachments/assets/bf4f0da1-1bdb-4196-90a4-7a5783efd6cf" />

- Kali Linux Attacker Machine - ip a
<img width="846" height="435" alt="Kali_Attacker_Machine_Network_Settings_ipa" src="https://github.com/user-attachments/assets/47a96b03-74da-4f3d-9d0d-f0714b003053" />

  
## Attack Simulation

- Hydra Bruteforce RDP
<img width="1262" height="586" alt="kali_hydra_bruteforce_windows10_server" src="https://github.com/user-attachments/assets/7d33852f-527c-447a-9214-680282e02900" />

- Nmap Port Scan on Windows 10 Server
<img src="https://i.imgur.com/5sWO6W8.png">

  
- Suricata
<img src="https://i.imgur.com/tsSikfa.png">

- Splunk Ingestion & Visualization
<img src="https://i.imgur.com/UVYlYas.png">

- Suricata Detection
<img src="https://i.imgur.com/pwK9aWY.png">
  
  
<br />

