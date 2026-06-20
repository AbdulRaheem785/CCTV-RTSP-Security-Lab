<p align="center">
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=00FF00&center=true&vCenter=true&width=900&lines=RTSP+Security+Assessment+Summary;CCTV+%2F+IP+Camera+Lab+Analysis;Network+Reconnaissance+%7C+Service+Enumeration;Controlled+Cybersecurity+Testing+Environment" />
</p>

---

<p align="center">

<img src="https://img.shields.io/badge/Project-RTSP_Lab-blue?style=for-the-badge">
<img src="https://img.shields.io/badge/Focus-CCTV_Security-red?style=for-the-badge">
<img src="https://img.shields.io/badge/Testing-Type_Controlled-green?style=for-the-badge">
<img src="https://img.shields.io/badge/Category-VAPT-orange?style=for-the-badge">
<img src="https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge">

</p>

---

## 📌 Project Overview

This document summarizes findings from a **controlled RTSP Security Assessment Lab** simulating IP camera and CCTV infrastructure in an isolated environment.

The objective was to analyze how exposed RTSP services behave under network reconnaissance and authentication testing, and to understand common security weaknesses in surveillance systems.

---

## 🧪 Scope of Assessment

- Network reconnaissance of CCTV/IP camera subnet  
- Service discovery (RTSP, SMB, HTTP)  
- RTSP stream enumeration  
- Authentication testing (controlled lab only)  
- Stream validation using media clients  
- Security posture analysis  

---

## 🛠️ Tools Used

- Nmap (Network Discovery & Port Scanning)  
- Python (Automation & Testing Scripts)  
- VLC Media Player (Stream Validation)  
- RTSP URI testing utilities  

---

## 🔍 Key Findings

### 1️⃣ Exposed RTSP Services
Multiple hosts exposed RTSP services, indicating video streaming interfaces were accessible over the network.

### 2️⃣ Weak or Missing Authentication
Some streams were accessible without proper authentication, showing misconfiguration risks.

### 3️⃣ Service Enumeration Possible
RTSP endpoints could be enumerated, allowing discovery of potential stream paths.

### 4️⃣ Attack Surface Exposure
Open services increased the attack surface and improved system discoverability via basic scanning.

---

## ⚠️ Security Risks Identified

- Unauthorized stream access risk  
- Exposure of surveillance feeds  
- Weak authentication configuration  
- Lack of network segmentation  
- Service enumeration leakage  

---

## 🛡️ Recommended Mitigations

- Enforce strong RTSP authentication (digest preferred)  
- Restrict camera access via VLAN segmentation  
- Disable unused services (HTTP / ONVIF if not required)  
- Apply firewall rules for RTSP (port 554)  
- Monitor logs for unauthorized access attempts  

---

## 📌 Conclusion

This lab demonstrates how misconfigured CCTV/IP camera systems can expose sensitive surveillance data when proper security controls are not implemented.

All testing was performed in a **controlled and authorized environment only** for educational cybersecurity learning purposes.
