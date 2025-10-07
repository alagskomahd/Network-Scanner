# 🌐 Network Scanner

A simple Python tool that discovers devices on a local network using ARP requests and lists IP and MAC addresses.  
Built for learning and safe network reconnaissance in controlled lab environments.

---

## 🎯 Objective
This project demonstrates basic LAN discovery using ARP. It helps learners understand how devices are discovered on a local network and how IP/MAC mappings are obtained.

---

## 🧩 Features
- Discover active hosts on a local IP range via ARP
- Return IP and MAC address pairs
- Lightweight and easy to run in lab environments

---

## ⚙️ Requirements
- **Operating System:** Linux / macOS (Linux recommended for packet-level access)  
- **Python:** 3.x (Python 3.10+ recommended)  
- **Python package:** `scapy`

> Install scapy:
> ```bash
> # using pip
> pip3 install scapy
> # on Debian/Ubuntu you may prefer the system package:
> sudo apt update && sudo apt install python3-scapy
> ```

---

## 🚀 Usage

1. **Clone this repository**
   ```bash
   git clone https://github.com/alagskomahd/network-scanner.git
   cd network-scanner
   
2. **You typically need root privileges to send/receive raw packets. Use sudo on Linux.**
   ```bash
   # Basic usage: scan a single IP or a network range (CIDR)
   sudo python3 network_scanner.py -t <ip range>

   # Or scan a single host
   sudo python3 network_scanner.py -t 192.168.1.10

3. **Example**
   ```bash
   sudo python3 network_scanner.py -t 192.168.1.0/24
   
3. **Expected Output**
   ```pgsql
   IP				        MAC Address
   ---------------------------------
   192.168.1.1          aa:bb:cc:dd:ee:ff
   192.168.1.12         11:22:33:44:55:66
   192.168.1.15         5d:2c:11:57:ff:33

🛡️ Safety & Ethics

This tool is for educational and authorized testing only. Only run scans on networks and machines you own or where you have explicit permission. Unauthorized scanning may be illegal and unethical.

---

🧾 Files in this repo

network_scanner.py — main script

README.md — this file

---

👤 Author

Dennis Alagskomah
📫 Email: alagskomah25@gmail.com
🔗 LinkedIn: https://www.linkedin.com/in/alagskomah/

