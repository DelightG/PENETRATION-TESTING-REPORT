# 🛡️ PENETRATION TESTING REPORT

### 🔎 FOOTPRINTING & NETWORK SCANNING PHASES

![Cybersecurity](https://img.shields.io/badge/CYBERSECURITY-NETWORKWALKS-0B3A6E?style=for-the-badge)
![Batch](https://img.shields.io/badge/BATCH-B084-D4A017?style=for-the-badge)
![Week](https://img.shields.io/badge/PROJECT-WEEK%2002-0B3A6E?style=for-the-badge)

### 👤 NDIDIAMAKA OKORIE

Cybersecurity Learner | Networkwalks Intern | Batch B084

---

## 🛡️ Engagement Overview

| Category | Details |
|---|---|
| 👤 Pentester | Ndidiamaka Okorie |
| 🎓 Program / Batch | B084 Networkwalks |
| 📅 Report Date | 13 November 2026 |
| 🧪 Modules | W2-PM1 Multiple Kali Tools |
| | W2-PM5 Zenmap Scanning |
| 🎯 Assessment Targets | Networkwalks Authorized Target |
| | My Own Local LAN Network |
| 🔐 Authorization | Authorized Educational Testing |
| 🔎 Phase 1 | Reconnaissance & Footprinting |
| 🌐 Phase 2 | Scanning & Network Discovery |
| 🚧 Phases 3–5 | Pending Further Practical Exercises |
| 🖥️ Primary Platforms | Kali Linux & Windows |

---

# 🛡️ 1. Liability & Authorization Disclaimer

> **AUTHORIZED SECURITY TESTING ONLY**

All activities documented in this report are intended for educational purposes, cybersecurity research, ethical hacking, and professional development.

Testing activities must only be performed against systems and devices for which appropriate authorization has been obtained.

Unauthorized access, scanning, enumeration, exploitation, or interference with computer systems may violate applicable laws and regulations.

The author, instructor, and Networkwalks are not responsible for misuse of the information contained in this project.

> 🛡️ Security Principle: Always define and respect the authorized scope before performing reconnaissance or security testing.

---

# 🛡️ 2. Introduction

This penetration testing report documents my practical cybersecurity activities during Week 2 of the Networkwalks Cybersecurity Training Program.

The assessment focuses on two major stages of the penetration testing lifecycle:

### 🔎 Phase 1: Reconnaissance & Footprinting

This phase involves gathering publicly available information about a target domain using different Kali Linux reconnaissance tools.

The tools used for this exercise include WHOIS, WhatWeb, Nslookup, cURL, Wafw00f, and DNSRecon.

### 🌐 Phase 2: Scanning & Network Discovery

This phase involves using Zenmap to identify active devices within my local network.

The exercise focuses on:

- Identifying the local IP address.
- Determining the network subnet.
- Discovering live hosts.
- Identifying IP addresses.
- Identifying MAC addresses.
- Visualizing network topology.

The practical exercises demonstrate the progression from:

```text
Public Information
       ↓
Reconnaissance
       ↓
Technology Identification
       ↓
DNS Enumeration
       ↓
Network Discovery
       ↓
Host Identification
       ↓
Network Topology
```

Each activity is documented with:

- 🖥️ Command or tool used.
- 📊 Observed results.
- 📸 Supporting evidence.
- 🔎 Security relevance.
- ⚠️ Potential risks.
- 🛡️ Recommended mitigation.

---

# 🛡️ 3. Tools & Technologies

| Tool / Technology | Purpose |
|---|---|
| 🐉 Kali Linux | Security testing and reconnaissance environment |
| 🪟 Windows | Local network identification |
| 🔍 WHOIS | Domain registration and name-server information |
| 🌐 WhatWeb | Web technology and CMS fingerprinting |
| 📡 Nslookup | DNS resolution and IP identification |
| 📥 cURL | HTTP response header analysis |
| 🛡️ Wafw00f | Web Application Firewall identification |
| 🗂️ DNSRecon | DNS record enumeration |
| 🛰️ Zenmap / Nmap | Network discovery and host scanning |
| 💻 Windows CMD | Local IP and MAC address identification |

---

# 🛡️ 4. Activities Performed

## 4.1 🔍 Footprinting & Reconnaissance

The first practical activity involved using Kali Linux reconnaissance tools to gather information about the authorized target domain.

The tools covered include:

```text
WHOIS
WhatWeb
Nslookup
cURL
Wafw00f
DNSRecon
```

Each tool provides a different perspective on publicly observable domain and web infrastructure information.

---

### 🔹 4.1.1 WHOIS

WHOIS was used to obtain publicly available domain registration information.

The activity helps identify information such as:

- Domain registrar.
- Domain registration details.
- Name servers.
- Registration and expiration information.

**Command:**

```bash
whois networkwalks.com
```

**Observed Results:**

[<img width="1920" height="1080" alt="W2-PM1-TASK 1 – WHOIS" src="https://github.com/user-attachments/assets/d8b26139-0360-4c5a-8998-745f84d461c1" />
]

**Security Relevance:**

WHOIS information provides an initial understanding of domain ownership and the infrastructure associated with a domain.

---

### 🔹 4.1.2 WhatWeb

WhatWeb was used to identify technologies and applications associated with the target website.

**Command:**

```bash
whatweb networkwalks.com
```

**Observed Results:**

[<img width="1920" height="1080" alt="W2-PM1-TASK 2 – WhatWeb" src="https://github.com/user-attachments/assets/d1787973-5ebb-4a49-bbf0-fb423f776556" />
]

**Security Relevance:**

Technology fingerprinting helps security professionals understand the technologies running on a website and identify software that may require further security review.

> 🛡️ Technology identification does not automatically mean that a vulnerability exists.

---

### 🔹 4.1.3 Nslookup

Nslookup was used to resolve the target domain name into its associated IP address.

**Command:**

```bash
nslookup networkwalks.com
```

**Observed Results:**

```text
Domain: networkwalks.com

IP Address: [INSERT ACTUAL IP ADDRESS]
```

**Security Relevance:**

DNS resolution provides information about the network location associated with a web service and supports further authorized infrastructure analysis.

---

### 🔹 4.1.4 cURL

cURL was used to inspect HTTP response headers returned by the target website.

**Command:**

```bash
curl -I networkwalks.com
```

**Observed Results:**

[<img width="960" height="540" alt="W2-PM1-TASK 4 – CURL" src="https://github.com/user-attachments/assets/227934f3-890e-4283-a7c0-cd2488656f31" />
]

**Security Relevance:**

HTTP response information can reveal technical details about a web application and help security professionals understand how a web server responds to requests.

---

### 🔹 4.1.5 Wafw00f

Wafw00f was used to identify whether a Web Application Firewall (WAF) protects the target website.

**Command:**

```bash
wafw00f https://networkwalks.com
```

**Observed Results:**

[<img width="960" height="540" alt="W2-PM1-TASK 5 – WAFW00F" src="https://github.com/user-attachments/assets/69ae4b2e-7e19-4940-822e-16d418e8ee1b" />
]

**Security Relevance:**

Identifying defensive technologies helps security professionals understand the security mechanisms protecting a web application.

---

### 🔹 4.1.6 DNSRecon

DNSRecon was used to gather publicly accessible DNS information associated with the target domain.

**Command:**

```bash
dnsrecon -d networkwalks.com
```

The activity focuses on identifying information such as:

- Name servers.
- Mail servers.
- SPF / TXT records.
- DNS records.
- Service records.

**Observed Results:**

[<img width="1920" height="1080" alt="W2-PM1-TASK 6 – DNSRecon" src="https://github.com/user-attachments/assets/7bde714c-5562-486f-9d77-0c08a714e626" />
]

**Security Relevance:**

DNS enumeration provides a broader understanding of an organization's publicly exposed infrastructure.

---

## 4.2 🌐 Network Scanning with Zenmap

The second practical activity focused on network discovery using Zenmap.

The objective was to identify devices connected to my local network and understand their network addresses.

The practical exercise involved:

- Identifying my computer's local IP address.
- Determining the subnet.
- Scanning the local network.
- Identifying live hosts.
- Collecting IP addresses.
- Identifying MAC addresses.
- Generating a network topology.

### 🔍 Step 1: Identifying Local Network Configuration

The Windows Command Prompt was used to retrieve network configuration details.

**Command:**

```cmd
ipconfig /all
```

The command provides information about:

- Hostname.
- IPv4 address.
- Subnet mask.
- Default gateway.
- Physical address (MAC address).
- DNS servers.

**My Network Configuration:**

| Network Information | Result |
|---|---|
| Computer Name | DESKTOP-RHKPJQD |
| IPv4 Address |192.168.56.1|
| Subnet Mask |255.255.255.0 |
| Default Gateway |  192.168.43.1 |
| Physical Address | 12:98:C3:1D:6B:89 |

### 🔍 Step 2: Network Scanning

Zenmap was used to perform a Ping Scan against my identified local subnet.

**Scan Type:**

```text
Ping Scan
```

**Target Network:**

```text
<img width="960" height="540" alt="Quick Scan" src="https://github.com/user-attachments/assets/fc8f1be6-8704-4050-bc56-7555f564c119" />

```

The scan was used to identify active devices responding within the authorized local network.

### 🛰️ Step 3: Live Hosts Identified

The scan results were used to identify active hosts within the network.
| No. | IP Address | MAC Address | Status |
|:---:|:---|:---|:---:|
| 1 | 192.168.43.1 | 12:98:C3:1D:6B:89 | 🟢 LIVE |
| 2 | 192.168.43.72 | 56:CA:EA:51:AC:B8 | 🟢 LIVE |
| 3 | 192.168.43.149 | 1A:89:C7:43:A6:4E | 🟢 LIVE |
| 4 | 192.168.43.14 | 94:B8:6D:38:9F:41 | 🟢 LIVE |
**Total Number of Live Hosts:** 4

### 🔍 Step 4: Network Topology

After completing the scan, the Topology section in Zenmap was used to visualize the discovered network.

The topology view helped illustrate the relationship between the scanning system and the discovered hosts.

The network topology was saved in PDF format as part of the practical evidence.

**Evidence:**

<img width="918" height="465" alt="Topology" src="https://github.com/user-attachments/assets/dbfd930d-172e-4c2f-b0e5-b450cfbb01c0" />


---

# 🛡️ 5. Risk Analysis & Impact

The following table provides a framework for documenting observations from the reconnaissance and network discovery activities.

| No. | Finding | Evidence / Observation | Potential Impact | Risk |
|---|---|---|---|---|
| 1 | Domain information exposure | WHOIS results | May reveal infrastructure information | To be assessed |
| 2 | Web technology identification | WhatWeb results | May assist technology fingerprinting | To be assessed |
| 3 | Server IP identification | Nslookup results | Reveals network location of web service | To be assessed |
| 4 | HTTP technical information | cURL results | May assist further enumeration | To be assessed |
| 5 | WAF identification | Wafw00f results | Reveals defensive technology | To be assessed |
| 6 | DNS information exposure | DNSRecon results | May assist infrastructure profiling | To be assessed |
| 7 | Live network hosts | Zenmap scan results | Unknown devices may represent unmanaged assets | To be assessed |

### Risk Rating Key

| Indicator | Severity |
|---|---|
| 🔴 | Critical |
| 🟠 | Medium |
| 🟢 | Low |
| ⚪ | Not Yet Assessed |

> **Important Assessment Note:** The identification of an IP address, DNS record, software version, or HTTP endpoint does not automatically confirm a security vulnerability. Further authorized testing is required to validate suspected vulnerabilities.

---

# 🛡️ 6. Recommendations

Based on the objectives of the assessment, the following security improvements are recommended.

### 1️⃣ Review Publicly Exposed Technology Information

Organizations should regularly review publicly exposed information relating to their CMS platforms, plugins, frameworks, and web technologies.

### 2️⃣ Maintain Updated Software

CMS platforms, plugins, frameworks, and other technologies should be regularly updated to address known security weaknesses.

### 3️⃣ Review HTTP Response Headers

HTTP response headers should be reviewed to determine whether unnecessary technical information is being exposed.

### 4️⃣ Review DNS Records

DNS records should be periodically reviewed to ensure that only necessary information and services are publicly exposed.

### 5️⃣ Properly Configure & Monitor the WAF

Web Application Firewalls should remain enabled, properly configured, monitored, and regularly updated.

### 6️⃣ Perform Regular Internal Network Discovery

Organizations should periodically scan authorized internal networks to identify active devices and maintain visibility of their infrastructure.

### 7️⃣ Investigate Unknown Devices

Unexpected devices identified during network discovery should be investigated and verified.

### 8️⃣ Maintain Network Documentation

Network topology, IP addresses, devices, and infrastructure documentation should be maintained and updated regularly.

### 9️⃣ Perform Security Testing Within an Authorized Scope

All reconnaissance, scanning, enumeration, and security testing should be conducted only against systems where appropriate authorization has been obtained.

---

# 🛡️ 7. Security Assessment Summary

| Assessment Area | Status |
|---|---|
| 🔎 Reconnaissance | Practical evidence to be documented |
| 🌐 Footprinting | Practical evidence to be documented |
| 🛰️ Network Discovery | Practical evidence to be documented |
| 🖥️ Host Identification | Results to be inserted |
| 🗺️ Network Topology | Evidence to be inserted |
| 💥 Exploitation | Not Performed |
| 🧪 Vulnerability Validation | Not Performed |
| 🚧 Advanced Testing | Pending |

### Overall Assessment

```text
RECONNAISSANCE
████████████████████  Practical exercise

FOOTPRINTING
████████████████████  Practical exercise

NETWORK DISCOVERY
████████████████████  Practical exercise

EXPLOITATION
░░░░░░░░░░░░░░░░░░░░  Not Performed
```

---

# 🛡️ 8. Key Learning Outcomes

Through these practical exercises, I developed knowledge and practical experience in:

- 🔎 Reconnaissance methodology.
- 🌐 Domain footprinting.
- 🧩 Web technology fingerprinting.
- 📡 DNS enumeration.
- 🛡️ Web Application Firewall identification.
- 🛰️ Network discovery.
- 🖥️ Host identification.
- 📍 IP and MAC address analysis.
- 🗺️ Network topology visualization.
- 📝 Professional security documentation.
- ⚖️ Authorized security testing principles.

The exercises demonstrated the importance of understanding a target environment before proceeding with further security testing.

They also reinforced the importance of documenting findings, understanding potential security risks, and recommending appropriate mitigation measures.

---

# 🛡️ 9. Conclusion

During Week 2 of my Cybersecurity Training Program at Networkwalks, I worked on practical activities covering reconnaissance, footprinting, and network scanning.

During the footprinting phase, I explored different Kali Linux tools for gathering publicly observable information about a target domain.

I learned the purpose of:

```text
WHOIS       → Domain registration information
WhatWeb     → Web technology fingerprinting
Nslookup    → DNS / IP resolution
cURL        → HTTP header inspection
Wafw00f     → WAF identification
DNSRecon    → DNS enumeration
```

During the network scanning phase, I used Windows Command Prompt and Zenmap to understand local network configurations, identify active hosts, examine IP and MAC addresses, and visualize network topology.

The exercises reinforced an important cybersecurity principle:

> Effective security testing begins with understanding the environment.

This project represents another step in my cybersecurity learning journey and contributes to my practical development in ethical hacking, network security, reconnaissance, and security assessment.

---

# 🛡️ 10. Evidence Collected

Evidence from the practical activities will be organized below.

### 🔎 Footprinting Evidence

| No. | Practical Activity | Evidence |
|---|---|---|
| 1 | WHOIS | <img width="1920" height="1080" alt="W2-PM1-TASK 1 – WHOIS" src="https://github.com/user-attachments/assets/cf5598da-65ae-4ada-ac3a-0b1cec45c09a" />

| 2 | WhatWeb | <img width="1920" height="1080" alt="W2-PM1-TASK 1 – WHOIS" src="https://github.com/user-attachments/assets/8c350479-7e35-475e-96d8-05c26d1c4215" />
|
| 3 | Nslookup | <img width="1920" height="1080" alt="W2-PM1-TASK 3 – NSLookup" src="https://github.com/user-attachments/assets/87af444b-1c28-4a83-9364-fa37361f47f2" />
 |
| 4 | cURL | <img width="960" height="540" alt="W2-PM1-TASK 4 – CURL" src="https://github.com/user-attachments/assets/3ac74f6e-a0c2-45ad-bfb2-a57e5c8d2d43" />
 |
| 5 | Wafw00f | <img width="960" height="540" alt="W2-PM1-TASK 5 – WAFW00F" src="https://github.com/user-attachments/assets/ce03b587-28e1-4711-8ea1-7f304761319d" />
 |
| 6 | DNSRecon | <img width="1920" height="1080" alt="W2-PM1-TASK 6 – DNSRecon" src="https://github.com/user-attachments/assets/44949309-707e-4b7b-9671-eaee93136583" />
 |

### 🌐 Zenmap Evidence

| No. | Practical Activity | Evidence |
|---|---|---|
| 1 |<img width="960" height="540" alt="Quick Scan" src="https://github.com/user-attachments/assets/db37f494-490f-4bbd-bd57-4df36c0deb1e" />

 |
| 2 | Zenmap Ping Scan | <img width="1920" height="1080" alt="Ipconfig" src="https://github.com/user-attachments/assets/d46eb205-034f-4887-b415-8d7cdd5470d2" />|
| 3 | Zenmap Host Discovery |<img width="960" height="540" alt="Host 4" src="https://github.com/user-attachments/assets/353863e0-8da7-40ad-87dc-0051d85e8d6a" />
|
| 4 | Zenmap Network Topology |<img width="918" height="465" alt="Topology" src="https://github.com/user-attachments/assets/e67ad256-6ed8-4a00-950c-eaf7d081118b" />
 |

### 📸 Evidence Folder Structure

```text
PENETRATION-TESTING-REPORT/
│
├── README.md
│
└── evidence/
    │
    ├── whois.png
    ├── whatweb.png
    ├── nslookup.png
    ├── curl.png
    ├── wafw00f.png
    ├── dnsrecon.png
    ├── ipconfig.png
    ├── zenmap-ping-scan.png
    ├── zenmap-host-discovery.png
    └── network-topology.pdf
```

---

# 🛡️ 11. Networkwalks Academy Quiz Assessment

As part of the Networkwalks Academy Cybersecurity Training Program, I am documenting my knowledge assessment covering cybersecurity concepts and the practical modules studied during the program.

### 🏆 Quiz Performance

| Assessment | Details |
|---|---|
| 🎓 Academy | Networkwalks Academy |
| 📚 Program | Cybersecurity |
| 📅 Assessment Date | [NOVEMBER 13|
| 🧪 Assessment Type | Knowledge Assessment |
| 📊 Score | [100%] |
| ✅ Result |<img width="960" height="540" alt="Practice Lab Score" src="https://github.com/user-attachments/assets/fdfe64b9-02f1-42e1-942e-0ac201ff495e" />
 |


### 🛡️ Learning Validation

The knowledge assessment provides an opportunity to evaluate my understanding of the cybersecurity concepts covered during the training and complements the hands-on practical activities documented in this repository.

Knowledge Assessment → Practical Lab → Evidence → Professional Documentation

---

# 🛡️ Assessment Progress

```text
PHASE 1
Reconnaissance & Footprinting
████████████████████████████████  PRACTICAL EXERCISE

PHASE 2
Scanning & Network Discovery
████████████████████████████████  PRACTICAL EXERCISE

PHASE 3
Vulnerability Assessment
░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  PENDING

PHASE 4
Exploitation
░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  PENDING

PHASE 5
Reporting & Remediation
░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░  IN PROGRESS
```

---

# 👤 Author

### NDIDIAMAKA OKORIE

Cybersecurity Learner | Networkwalks Intern | Batch B082

---

# 🛡️ Project Information

| Project Detail | Information |
|---|---|
| 🏢 Program | Cybersecurity Program – Networkwalks |
| 📅 Week | Week 02 |
| 🎓 Batch | B084|
| 🔐 Project Type | Authorized Penetration Testing Lab |
| 🔎 Primary Focus | Footprinting & Network Scanning |
| 🐉 Primary OS | Kali Linux |
| 🛰️ Scanning Tool | Zenmap / Nmap |
| 📊 Assessment Status | Practical Documentation |
| 📁 Repository | GitHub |

---

### 🛡️ CYBERSECURITY • ETHICAL HACKING • NETWORK SECURITY

**Learn → Practice → Analyze → Secure**

W2-PM-FINAL | Networkwalks | B084| November 2026

---

**END OF REPORT**
