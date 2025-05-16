# Security Assessment Report

Welcome to the official repository for my graduation project submitted as part of the **Digital Egyptian Pioneers Initiative (DEPI)** in the **Infrastructure Cybersecurity** track.

## 📌 Project Overview

As part of DEPI, my team and I were tasked with simulating a full security assessment engagement for a fictional software engineering company we created from scratch, called **CodeByte Technologies**.

Instead of building a physical environment, we strategically pieced together a realistic network using machines and rooms from **Hack The Box** and **TryHackMe**. Our setup included public-facing web servers, a production development network, and a full internal **Active Directory** domain—mimicking what you’d expect in a real company network.

This repository includes the deliverables from that engagement.

---

## 🛠️ Penetration Testing Phases

### 🌐 External Penetration Testing

| Machine Name          | Platform     | Vulnerability Code(s)         | Description                             |
|----------------------|--------------|-------------------------------|-----------------------------------------|
| Keeper               | Hack The Box | EPT-001, EPT-002, EPT-003     | Default credentials, cleartext passwords, outdated KeePass exploitation |
| Titanic              | Hack The Box | EPT-004, EPT-005, EPT-006     | Path traversal, Git repo exposure, ImageMagick RCE |
| Writeup              | Hack The Box | EPT-007, EPT-008              | Blind SQL Injection, Path Hijacking     |
| Beep                 | Hack The Box | EPT-009                       | Directory Traversal                     |
| Thomas Wreath (Wreath) | TryHackMe   | EPT-010                       | MiniServ RCE (Outdated Software)        |
| Jack                 | TryHackMe    | EPT-011, EPT-012, EPT-013     | Brute force via XML-RPC, parameter tampering, vulnerable cron job |

### 🖥️ Internal Penetration Testing
The internal penetration test was simulated with the Wreath and Attacktive Directory rooms on TryHackme.

| Host / Component     | Vulnerability Code(s)         | Description                             |
|----------------------|-------------------------------|-----------------------------------------|
| Git Server (10.200.81.150) | IPT-001, IPT-002, IPT-003, IPT-004, IPT-005, IPT-006 | Error page info disclosure, GitStack RCE, SYSTEM privilege service, undetected admin account, no AV, weak password policy |
| Wreath-PC (10.200.81.100)  | IPT-007, IPT-008, IPT-009   | Unrestricted file upload, info leakage via code comments, unquoted service path |
| Domain Controller (10.10.254.39) | IPT-010, IPT-011, IPT-012 | Kerberoasting, insecure credential storage, domain admin privilege abuse |

---

## 📄 Deliverables

### 🔐 Security Assessment Report (SAR)
A comprehensive 79-page document detailing:

- Executive summary
- External and internal attack walkthroughs
- Vulnerability severities
- Proof-of-concepts with screenshots
- Tools used
- Recommended mitigation strategies for every finding

📁 File: `SAR.pdf`

### 🧾 Project Overview
Outlines the scope of the project, team responsibilities, selected boxes/rooms, and key learning outcomes.

📁 File: `DEPI Graduation Project Overview.pdf`

---

## 👨‍💻 My Role

- Designed the project structure 
- Conducted the **entire internal penetration test**
- Led the **documentation effort** by creating the full Security Assessment Report
- Consolidated findings from all team members into a professional-grade deliverable

---

## 🧠 What I Learned

This project gave me hands-on experience in:
- Simulating real-world enterprise networks
- Performing end-to-end penetration testing engagements
- Using tools like Nmap, Burp Suite, Chisel, Evil-WinRM, Mimikatz, Hashcat, and more
- Writing detailed, actionable security documentation that aligns with frameworks like **NIST SP 800-115** and **OWASP**

---

## 🤝 Credits

Big thanks to the amazing team:  
- **Khaled Shaaban**  
- Abdelrahman Tarek  
- Abd Elrhman Emad  
- Eslam Salem  
- Mohamed Ali  
- Sandra Adel  

And a special thank-you to the mentors and organizers of **DEPI** for their guidance and support throughout the journey.

---



## 🔐 Disclaimer

All testing was performed in legal, simulated environments. No real systems or organizations were harmed or compromised during this project.
