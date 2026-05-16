# 🔐 Vulnerability Assessment Report — Task 1

## 📌 Project Overview

This project is part of the Cyber Security Internship program at Future Interns.

The objective of this task was to perform a **basic vulnerability assessment (read-only scope)** on a public web application and document findings in a professional security report.

The focus was on identifying common security misconfigurations and exposure risks using passive analysis techniques only.

---

## 🌐 Target Website

- OWASP Juice Shop Demo  
- https://demo.owasp-juice.shop

---

## 🎯 Objectives

- Perform passive security analysis of a public web application
- Identify common security misconfigurations
- Classify risks (Low / Medium / High)
- Provide clear remediation recommendations
- Document findings in a professional format

---

## 🛠️ Tools Used

- Nmap (Service & port enumeration)
- OWASP ZAP (Passive scan only)
- Browser Developer Tools (Header inspection)
- Linux (Kali environment)
- GitHub (documentation & version control)

---

## 🔍 Methodology

1. Performed service and port scanning using Nmap
2. Conducted passive analysis using OWASP ZAP
3. Inspected HTTP security headers using browser DevTools
4. Collected and documented security findings
5. Classified risks based on business impact

---

## ⚠️ Key Findings

### 1. CORS Misconfiguration
- **Risk Level:** Medium  
- Access-Control-Allow-Origin set to wildcard (*) in some responses  
- Could allow unauthorized cross-origin access

### 2. Server Information Disclosure
- **Risk Level:** Low  
- Server reveals infrastructure details (Heroku, Apache)

### 3. API & Socket.io Exposure
- **Risk Level:** Medium  
- Real-time communication endpoints exposed without strict control

### 4. Security Headers Present (Positive Finding)
- X-Frame-Options enabled  
- X-Content-Type-Options enabled  
- Helps reduce client-side attack risks

---

## 🧾 Risk Summary

- 🔴 High: 0
- 🟠 Medium: 2
- 🟢 Low: 1
- 🔵 Info/Positive: 1

Overall security posture: **Moderate with misconfiguration risks**

---

## 💡 Recommendations

- Restrict CORS policy to trusted domains only
- Hide server and technology stack details
- Secure real-time communication endpoints (auth + rate limiting)
- Continue enforcing security headers
- Perform regular vulnerability assessments

---

## 📁 Repository Structure

