# 🛡️ Cyber Security Assignment 1
---

## 👥 Group Members
- **PHRINCE POWLGREAT DIDYMUS** (25030698)  
- **NAVIN RAMAIAH** (25030584)  
---

## 📂 Table of Contents
1. Introduction  
2. Reconnaissance Tools  
   - Nmap  
   - DNSRecon  
   - Hping3  
3. Maintaining Access Tools  
   - Cryptcat  
   - Weevely  
   - Metasploit  
4. Comparison & Conclusions  
5. References  

---

## 🔎 Introduction
This assignment demonstrates reconnaissance and maintaining access using **Kali Linux tools** in a controlled VirtualBox environment.  
* Reconnaissance tools: Nmap, DNSRecon, Hping3  
* Maintaining access tools: Cryptcat, Weevely, Metasploit  

Screenshots were taken during testing, with sensitive information blacked out.

---

## 🕵️ Reconnaissance Tools

### 1. Nmap
**Features tested:**
* Basic port scan (`nmap localhost`)  
* Service/version detection (`nmap -sV localhost`)  
* Aggressive scan with OS detection (`nmap -A localhost`)  

**Screenshots:**  
![Nmap Basic Scan](https://github.com/NavinRamaiah/Cyber-Security-/blob/main/WhatsApp%20Image%202026-02-28%20at%2010.32.18%20AM.jpeg) 
![Nmap Service Detection](https://github.com/NavinRamaiah/Cyber-Security-/blob/main/WhatsApp%20Image%202026-02-28%20at%2010.32.18%20AM%20(1).jpeg)  
![Nmap Aggressive Scan](https://github.com/NavinRamaiah/Cyber-Security-/blob/main/WhatsApp%20Image%202026-02-28%20at%2010.32.19%20AM.jpeg)

---

### 2. DNSRecon
**Features tested:**
* Domain resolution (`nslookup google.com`)  
* DNS record enumeration (`dnsrecon -d google.com`)  
* Subdomain brute force (`dnsrecon -d google.com -t brt`)  

**Screenshots:**  
![DNSRecon Lookup](https://github.com/NavinRamaiah/Cyber-Security-/blob/main/WhatsApp%20Image%202026-02-28%20at%2010.32.19%20AM%20(1).jpeg)  
![DNSRecon Enumeration](https://github.com/NavinRamaiah/Cyber-Security-/blob/main/WhatsApp%20Image%202026-02-28%20at%2010.32.20%20AM.jpeg)  
![DNSRecon Subdomains](https://github.com/NavinRamaiah/Cyber-Security-/blob/main/WhatsApp%20Image%202026-02-28%20at%2011.27.33%20AM.jpeg)

---

### 3. Hping3
**Features tested:**
* ICMP ping (`hping3 -1 localhost`)  
* TCP SYN scan (`hping3 -S -p 80 google.com`)  
* UDP test (`hping3 -2 -p 53 google.com`)  

**Screenshots:**  
![Hping3 ICMP](screenshots/hping3_icmp.png)  
![Hping3 TCP SYN](https://github.com/NavinRamaiah/Cyber-Security-/blob/main/WhatsApp%20Image%202026-02-28%20at%2010.32.21%20AM.jpeg)  
![Hping3 UDP](https://github.com/NavinRamaiah/Cyber-Security-/blob/main/WhatsApp%20Image%202026-02-28%20at%2010.32.21%20AM%20(1).jpeg)

---

## 🔐 Maintaining Access Tools

### 1. Cryptcat
**Features tested:**
* Listener setup (`cryptcat -l -p 4444`)  
* Client connection (`cryptcat 127.0.0.1 4444`)  
* Encrypted bidirectional communication  

**Screenshots:**  
![Cryptcat Listener](screenshots/cryptcat_listener.png)  
![Cryptcat Connection](screenshots/cryptcat_connection.png)

---

### 2. Weevely
**Features tested:**
* Generate PHP backdoor (`weevely generate password123 shell.php`)  
* Host shell with PHP server (`php -S 127.0.0.1:8000`)  
* Remote command execution (`weevely http://127.0.0.1:8000/shell.php password123`)  

**Screenshots:**  
![Weevely Shell Generated](screenshots/weevely_generate.png)  
![Weevely Connection](screenshots/weevely_connect.png)  
![Weevely Commands](screenshots/weevely_commands.png)

---

### 3. Metasploit
**Features tested:**
* Launch framework (`msfconsole`)  
* Configure handler (`use exploit/multi/handler`)  
* Reverse shell payload setup (`set payload generic/shell_reverse_tcp`)  

**Screenshots:**  
![Metasploit Console](screenshots/metasploit_console.png)  
![Metasploit Handler](screenshots/metasploit_handler.png)  
![Metasploit Payload](screenshots/metasploit_payload.png)

---

## 📊 Comparison & Conclusions

### Reconnaissance Tools
* **Nmap**: Automated port/service scanning, OS detection.  
* **DNSRecon**: Domain-level enumeration, DNS records, subdomains.  
* **Hping3**: Protocol-level testing with ICMP, TCP, UDP.  

### Maintaining Access Tools
* **Cryptcat**: Simple encrypted TCP communication.  
* **Weevely**: Web-based backdoor with HTTP traffic blending.  
* **Metasploit**: Structured exploitation framework with session management.  

**Conclusion:**  
Reconnaissance tools gather intelligence before exploitation, while maintaining access tools ensure persistence after exploitation. Together, they form a complete penetration testing workflow.

---

## 📚 References
* Nmap Documentation – [Nmap.org](https://nmap.org/book/man.html)  
* DNSRecon GitHub – [DNSRecon Repository](https://github.com/darkoperator/dnsrecon)  
* Hping3 Manual – [Kali Linux Tools: Hping3](https://www.kali.org/tools/hping3/)  
* Cryptcat Documentation – [Cryptcat SourceForge](http://cryptcat.sourceforge.net/)  
* Weevely GitHub – [Weevely Repository](https://github.com/epinna/weevely3)  
* Metasploit Documentation – [Rapid7 Metasploit Docs](https://docs.rapid7.com/metasploit/)  ps://docs.rapid7.com/metasploit/)  
- Weevely GitHub – [Weevely Repository](https://github.com/epinna/weevely3)  
- Cryptcat Documentation – [Cryptcat Manual](http://cryptcat.sourceforge.net/)  
