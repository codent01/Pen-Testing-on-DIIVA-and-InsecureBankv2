<h1 align="center">🛡️ Offensive Security in Mobile Applications</h1>
<p align="center">
  <strong>Penetration Testing on DIVA & InsecureBankv2</strong><br/>
  A comprehensive security assessment of Android mobile apps — covering static analysis, dynamic testing, buffer overflows, CVE analysis, and Red Team vs Blue Team simulations.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Metasploit-2596CD?style=for-the-badge&logo=metasploit&logoColor=white"/>
  <img src="https://img.shields.io/badge/Frida-FF6633?style=for-the-badge"/>
  <img src="https://img.shields.io/badge/Burp_Suite-FF6633?style=for-the-badge&logo=burpsuite&logoColor=white"/>
  <img src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white"/>
</p>

---

## Overview

This project demonstrates a full offensive security assessment of mobile applications, targeting **DIVA (Damn Insecure and Vulnerable App)** and **InsecureBankv2** — two intentionally vulnerable Android apps used for security training. The assessment covers the complete pen-testing lifecycle from reconnaissance to exploitation to reporting.

---

## Key Areas

### 🔍 Platform-Specific Analysis
- Android-specific vulnerabilities: Fragment Injection, WebView exploits, insecure data storage
- iOS challenges: Jailbreak detection bypass, Keychain analysis
- Cross-platform: Network communication, authentication, and data storage flaws

### 🧪 Static Analysis
APK decompilation and code review using `jadx-gui`, `apktool`, and `dex2jar` to identify hardcoded secrets, insecure configurations, and vulnerable code patterns.

### ⚡ Dynamic Analysis
Runtime testing with **Frida** for method hooking, SSL pinning bypass, and real-time behavior monitoring. Network interception via **Burp Suite**.

### 💥 Buffer Overflow Exploitation
Advanced memory handling attack simulations using **Metasploit** for payload generation and custom exploit development. Vulnerability scanning with **Nessus**.

### 🔐 CVE & CWE Analysis
Evaluation of real-world vulnerabilities including:
- **CVE-2023-21002** — Android-specific security flaw
- **CWE-89** — SQL Injection
- **CWE-79** — Cross-Site Scripting (XSS)

### 🔴🔵 Red Team vs Blue Team Simulation
- **Offensive**: SQL Injection, XSS, password attacks, privilege escalation
- **Defensive**: MFA implementation, RBAC, SIEM deployment, incident response

---

## Tools & Technologies

| Category | Tools |
|----------|-------|
| **Languages** | Python, Java |
| **Exploitation** | Metasploit Framework |
| **Instrumentation** | Frida |
| **Scanning** | Nessus |
| **Proxy** | Burp Suite |
| **Static Analysis** | jadx-gui, apktool, dex2jar |
| **Environment** | Android Studio, ADB |
| **Reporting** | Python (ReportLab PDF generation) |

---

## Project Structure

```
Pen-Testing/
├── android_pentest.py              # Android penetration testing script
├── diva_security_report.py         # DIVA vulnerability analysis
├── insecurebank_analysis.py        # InsecureBankv2 security assessment
├── buffer_overflow_report_gen.py   # Buffer overflow exploit report
├── red_team_simulation.py          # Red Team attack simulation
├── advanced_redblue_report.py      # Red/Blue Team comparison report
├── generate_detailed_pdf_report.py # Comprehensive PDF report generator
├── requirements.txt                # Python dependencies
├── DIVA_Security_Report.pdf        # Generated DIVA report
├── RedTeam_Simulation_Report.pdf   # Red Team findings
└── README.md
```

---

## Getting Started

### Prerequisites
- Python 3.9+
- Android Studio with emulator
- Security tools: Metasploit, Frida, Burp Suite

### Installation

1. **Clone the repo**
   ```bash
   git clone https://github.com/codent01/Pen-Testing-on-DIIVA-and-InsecureBankv2.git
   cd Pen-Testing-on-DIIVA-and-InsecureBankv2
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up test environment**
   - Deploy **InsecureBankv2** APK on an Android emulator
   - Configure **DIVA** app for testing

4. **Run analysis**
   ```bash
   python android_pentest.py
   python diva_security_report.py
   ```

---

## Reports

Pre-generated PDF reports are included:
- `DIVA_Security_Report.pdf` — Full vulnerability assessment of DIVA
- `RedTeam_Simulation_Report.pdf` — Red Team exercise findings
- `Red_Team_Assessment_*.pdf` — Detailed Red Team assessment

---

## Roadmap

- [x] DIVA vulnerability assessment
- [x] InsecureBankv2 penetration testing
- [x] Buffer overflow exploitation
- [x] CVE/CWE analysis
- [x] Red vs Blue Team simulation
- [x] Automated PDF report generation
- [ ] ML-based threat detection
- [ ] Additional CVE coverage
- [ ] Security training modules

---

<p align="center">
  <i>Understanding attacks is the first step to building better defenses.</i><br/>
  <strong>Analyze. Exploit. Secure.</strong>
</p>
