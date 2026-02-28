# 🛡️ Cyber Security Assignment 1
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

Each tool was tested with at least **three features**, and screenshots were taken to demonstrate usage. Sensitive information such as IP addresses and domains has been blacked out.

---

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
![Nmap Result](screenshots/nmap_result.png)

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

---

## 🔐 Maintaining Access Tools

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

---

## 📊 Comparison & Conclusions
- **Reconnaissance tools** focus on **information gathering** (ports, services, DNS records).  
- **Maintaining access tools** focus on **persistence and stealth** (backdoors, encrypted communication, reverse shells).  
- Recon-ng and Nmap are structured and widely used for scanning, while tools like Weevely and Cryptcat are lightweight but effective for persistence.  
- Overall, combining reconnaissance and persistence tools provides a **complete penetration testing workflow**.  

---

## 📚 References
- Recon-ng Documentation  
- Nmap Official Guide  
- Hping3 Manual  
- DNSRecon GitHub  
- Metasploit Documentation  
- Weevely GitHub  
- Cryptcat Documentation  
