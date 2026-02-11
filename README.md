# Nmap Network Scanning Report

## 🔎 Target Information
Target: scanme.nmap.org  
Scan Type: Full Port Scan + Service Detection  
Tool Used: Nmap  
Operating System: Kali Linux  

---

## 📡 Scan Command Used

nmap -sS -sV -O -T4 -p- scanme.nmap.org -oA pro_scan

---

## 🖥 Open Ports & Services Found

| Port | State | Service | Version |
|------|-------|----------|----------|
| 22   | Open  | SSH      | OpenSSH |
| 80   | Open  | HTTP     | Apache |

---

## ⚠ Risk Analysis

- Port 22 (SSH):  
  If weak password is used, attacker can attempt brute force attack.

- Port 80 (HTTP):  
  Web server should be checked for outdated software or vulnerabilities.

---

## 🛡 Security Recommendations

- Use strong passwords for SSH
- Disable root login via SSH
- Keep Apache updated
- Use firewall to restrict unnecessary ports

---

## 📁 Files Included

- pro_scan.nmap
- pro_scan.xml
- pro_scan.gnmap

---

## 📌 Conclusion

The scan successfully identified open ports and running services.  
Further vulnerability assessment is recommended.
