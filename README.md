# RedTeam-OT
# 🔍 OT Red Teaming Tools for Power & Energy Sectors

## 🚀 Overview
This repository contains a curated list of **open-source tools** for **OT (Operational Technology) red teaming** in **power and energy sectors**. These tools assist in **scanning, identifying, and exploiting vulnerabilities** in industrial control systems (ICS) and SCADA environments. 

## 📌 Categories
- 🔍 **OT Network Discovery & Scanning**
- 🎯 **OT Vulnerability Identification & Exploitation**
- 📡 **Protocol-Specific Tools (Modbus, DNP3, IEC 61850, BACnet, Siemens S7, etc.)**
- 🛠 **Adversary Emulation & Attack Simulation**
- 🏭 **PLC & Device Fingerprinting Tools**
- 📖 **Documentation & Learning Resources**

---

## 🔍 1. OT Network Discovery & Scanning

### 1️⃣ **Redpoint (Nmap ICS Scripts)**
📌 **Description**: A collection of **Nmap NSE scripts** designed for discovering and fingerprinting ICS/SCADA devices.

📌 **Features**:
- Identifies **Modbus, DNP3, BACnet, Ethernet/IP, Siemens S7, IEC 61850 devices**
- Extracts **firmware, device type, and open ports**
- Helps in **network reconnaissance**

📌 **GitHub**: [Redpoint Nmap Scripts](https://github.com/digitalbond/Redpoint)

📌 **Usage**:
```bash
nmap --script modbus-discover,dnp3-info,bacnet-info,s7-info -p 502,20000,47808,102 <TARGET_IP>
```

---

### 2️⃣ **PLCScan**
📌 **Description**: A fast **PLC scanner for discovering Siemens S7 and Modbus devices**.

📌 **Features**:
- Detects **Siemens S7 PLCs and Modbus devices**
- Extracts firmware, model type, and available services

📌 **GitHub**: [PLCScan](https://github.com/Faxm0dem/PLCscan)

📌 **Usage**:
```bash
python3 plcscan.py --ip <TARGET_IP>
```

---

### 3️⃣ **ModScan**
📌 **Description**: A **Modbus/TCP device scanner** that identifies Modbus assets and enumerates accessible registers.

📌 **GitHub**: [ModScan](https://github.com/moki-ics/modscan)

📌 **Usage**:
```bash
modscan -t <TARGET_IP> -p 502
```

---

### 4️⃣ **GrassMarlin (NSA)**
📌 **Description**: **Passive ICS network monitoring tool** that maps out OT assets without active scanning.

📌 **GitHub**: [GrassMarlin](https://github.com/nsacyber/GRASSMARLIN)

📌 **Usage**:
```bash
grassmarlin
```

---

## 🎯 2. OT Vulnerability Identification & Exploitation

### 5️⃣ **Metasploit (ICS Modules)**
📌 **Description**: Open-source **penetration testing framework** with **ICS/SCADA exploit modules**.

📌 **GitHub**: [Metasploit](https://github.com/rapid7/metasploit-framework)

📌 **Usage**:
```bash
msfconsole
use exploit/scada/modbus
```

---

### 6️⃣ **Industrial Exploitation Framework (ISF)**
📌 **Description**: A **Python-based ICS exploitation toolkit** similar to Metasploit but focused on **industrial controllers**.

📌 **GitHub**: [ISF](https://github.com/dark-lbp/isf)

📌 **Usage**:
```bash
python3 isf.py
```

---

## 📡 3. Protocol-Specific Tools (Modbus, DNP3, IEC 61850, etc.)

### 7️⃣ **ModbusPwn**
📌 **Description**: A **Modbus/TCP exploitation toolkit** with scanning and attack modules.

📌 **GitHub**: [ModBusPwn](https://github.com/InfoSec-DB/ModBusPwn)

📌 **Usage**:
```bash
python3 modbuspwn.py --scan <TARGET_IP>
```

---

### 8️⃣ **OpenDNP3**
📌 **Description**: Open-source **DNP3 protocol library** used for fuzzing and testing industrial controllers.

📌 **GitHub**: [OpenDNP3](https://github.com/dnp3/opendnp3)

---

## 🏭 4. PLC & Device Fingerprinting Tools

### 9️⃣ **S7Scan**
📌 **Description**: A **Siemens PLC scanner** that extracts model details and security configurations.

📌 **GitHub**: [S7Scan](https://github.com/SCADAStrangelove)

📌 **Usage**:
```bash
python3 s7scan.py -i <TARGET_IP>
```

---

### 🔟 **Snap7**
📌 **Description**: A library for interacting with **Siemens S7 PLCs**, allowing read/write access to data blocks.

📌 **GitHub**: [Snap7](https://sourceforge.net/projects/snap7)

---

## 🔗 5. Adversary Emulation & Attack Simulation

### 🔥 **MITRE Caldera for OT**
📌 **Description**: **Adversary emulation framework** with **pre-built attack scripts** for OT.

📌 **GitHub**: [MITRE Caldera for OT](https://github.com/mitre/caldera-ot)

📌 **Usage**:
```bash
python3 caldera.py
```

---

## 📖 6. Documentation & Learning Resources

- **ICS-CERT Training (CISA)** – Free ICS security training from **CISA/DHS** ([ICS-CERT Training](https://ics-cert.us-cert.gov/Training))
- **MITRE ATT&CK for ICS** – Adversary techniques for **SCADA/ICS attacks** ([MITRE ATT&CK ICS](https://attack.mitre.org/matrices/ics/))
- **Awesome ICS Security** – Curated ICS security resources ([Awesome ICS Security](https://github.com/ITI/awesome-ics-security))

---

## 🚀 Contributing
If you have **new tools** or updates, feel free to submit a **Pull Request**! 

---

## ⚠️ Disclaimer
🚨 **For educational and authorized security research purposes only!** Use these tools only on **systems you own or have explicit permission to test.** Misuse may lead to legal consequences. 🚨

---
---

### 🌟 Star this repo if you found it useful! ⭐
