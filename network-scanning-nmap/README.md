# 🔍 Network Scanning and Enumeration with Nmap

## 📝 Project Summary
In this project, I used **Nmap** to scan and enumerate a target machine running in my virtual lab. This is a common task for both cybersecurity defenders and ethical hackers to identify open ports, services, and potential vulnerabilities.

---

## 🧰 Tools Used
- 🧪 **Kali Linux** (in VirtualBox)
- 🎯 **Metasploitable 2** (as target machine)
- 📡 **Nmap** (network mapping and scanning tool)

---

## 🛠️ Steps Taken

### Step 1: Lab Setup
- Installed Kali Linux and Metasploitable 2 in VirtualBox.
- Placed both on **Host-Only Network** so they could talk to each other.

### Step 2: Ping the Target
```bash
ping [Metasploitable IP]
nmap [target IP]
nmap -sV [target IP]
nmap -A [target IP]
