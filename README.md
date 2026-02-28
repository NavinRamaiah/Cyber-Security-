# 🛡️ Cyber Security Assignment 1
---

## 👥 Group Members
- **PHRINCE POWLGREAT DIDYMUS** (25030698)  
- **NAVIN RAMAIAH** (25030584)  
---

## 📂 Table of Contents
1. Introduction  
2. Reconnaissance Tools  
   - Recon-ng  
   - Nmap  
   - Hping3  
   - DNSRecon  
3. Maintaining Access Tools  
   - Metasploit  
   - Weevely  
   - Cryptcat  
4. Comparison & Conclusions  
5. References  

---

## 🔎 Introduction
In this assignment, I explored **Kali Linux tools** for two phases of penetration testing:  
- **Reconnaissance** (information gathering)  
- **Maintaining Access** (persistence after exploitation)
## 🕵️ Reconnaissance Tools

### 1. Recon-ng
**Features tested:**
- Workspace creation  
- Module usage for domain reconnaissance  
- Exporting results  

**Screenshots:**  
![Recon-ng Result](screenshots/reconng_result.png)

---

### 2. Nmap
**Features tested:**
- Port scanning  
- Service/version detection  
- OS fingerprinting  

**Screenshots:**
![Nmap Result](WhatsApp%20Image%202026-02-28%20at%2020.58.00.png)

---

### 3. Hping3
**Features tested:**
- TCP SYN scan  
- ICMP ping  
- Traceroute functionality  

**Screenshots:**  
![Hping3 Result](screenshots/hping3_result.png)

---

### 4. DNSRecon
**Features tested:**
- Standard DNS enumeration  
- Zone transfer testing  
- Reverse lookup  

**Screenshots:**  
![DNSRecon Result](screenshots/dnsrecon_result.png)
- ## 🔐 Maintaining Access Tools

### 1. Metasploit
**Features tested:**
- Exploit execution  
- Meterpreter session management  
- Persistence module  

**Screenshots:**  
![Metasploit Result](screenshots/metasploit_result.png)

---

### 2. Weevely
**Features tested:**
- Generating a backdoor  
- Remote command execution  
- Privilege escalation attempts  

**Screenshots:**  
![Weevely Result](screenshots/weevely_result.png)

---

### 3. Cryptcat
**Features tested:**
- Encrypted communication  
- Reverse shell setup  
- File transfer  

**Screenshots:**  
![Cryptcat Result](screenshots/cryptcat_result.png)

## 📊 Comparison & Conclusions

### Reconnaissance Tools
- **Recon-ng** provided a structured framework for domain reconnaissance, making it easy to organize results.  
- **Nmap** was the most versatile, offering port scanning, service detection, and OS fingerprinting in one tool.  
- **Hping3** allowed packet‑level testing, useful for simulating different types of traffic.  
- **DNSRecon** specialized in DNS enumeration, zone transfer testing, and reverse lookups.

**Conclusion:** Reconnaissance tools focus on **information gathering**. They help identify open ports, services, DNS records, and potential attack surfaces before exploitation.

---

### Maintaining Access Tools
- **Metasploit** offered advanced persistence modules and session management, making it powerful for long‑term access.  
- **Weevely** was lightweight and effective for generating PHP backdoors and executing remote commands.  
- **Cryptcat** enabled encrypted communication and reverse shells, ensuring stealth and secure persistence.

**Conclusion:** Maintaining access tools focus on **persistence and stealth**. They allow attackers to remain inside a system after exploitation, often bypassing detection through encryption or covert channels.

---

### Overall Comparison
- Reconnaissance tools are **proactive**: they gather intelligence before exploitation.  
- Maintaining access tools are **reactive**: they ensure persistence after exploitation.  
- Combining both phases provides a **complete penetration testing workflow** — from discovery to persistence.  
- Tools like **Nmap + Metasploit** form the backbone of many penetration tests, while **Weevely and Cryptcat** demonstrate lightweight but effective persistence techniques.

---
## 📚 References
- Recon-ng Documentation – [HackerTarget Recon-ng Tutorial](https://hackertarget.com/recon-ng-tutorial)   
- Nmap Official Guide – [Nmap.org Documentation](https://nmap.org/book/man.html)  
- Hping3 Manual – [Kali Linux Tools: Hping3](https://www.kali.org/tools/hping3/)   
- DNSRecon GitHub – [DNSRecon Repository](https://github.com/darkoperator/dnsrecon)  
- Metasploit Documentation – [Rapid7 Metasploit Documentation](https://docs.rapid7.com/metasploit/)  
- Weevely GitHub – [Weevely Repository](https://github.com/epinna/weevely3)  
- Cryptcat Documentation – [Cryptcat Manual](http://cryptcat.sourceforge.net/)  
