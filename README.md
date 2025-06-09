# pasta-threat-modeling

# 🧠 Threat Modeling with PASTA: Stages Sneaker Company

This project applies the **PASTA (Process for Attack Simulation and Threat Analysis)** framework to a fictional e-commerce platform called **Stages Sneaker Company**. The goal is to identify, evaluate, and propose mitigations for threats across the platform's architecture using the 7-stage PASTA model.

---

## 📌 Business & Security Objectives

- Maintain the **confidentiality, integrity, and availability (CIA)** of customer data
- Improve user experience by streamlining signup, login, and account management
- Enable secure, fast, and flexible payment options during checkout

---

## 🧱 Technical Scope

Technologies used:
- **API**
- **Public Key Infrastructure (PKI)**
- **AES** (Advanced Encryption Standard)
- **SHA-256** (Secure Hash Algorithm)
- **SQL** (noted as highest-priority risk)

**Primary concern:** SQL injection threats — input sanitization and prepared statements are needed to mitigate this risk. Codebase and user input pathways require inspection for vulnerabilities.

---

## 🔍 Threat & Vulnerability Analysis

### Threats Identified
- **Social engineering** targeting employees to gain access to internal assets
- **SQL injection**, including:
  - In-band
  - Out-of-band
  - Inferential injection

### Vulnerabilities
- Lack of secure input validation on user fields
- Risk of compromised credentials via phishing/social engineering
- Incomplete authentication control mechanisms

---

## 🧩 Attack Modeling

- Developed **attack trees** to simulate pathways used to exploit the system
- Used sample data flow and diagramming to map attack surfaces

---

## 🛡 Risk Mitigation Plan

- Implement **prepared statements** and **input sanitization** on all user input fields  
- Provide **employee training** on phishing and social engineering  
- Enforce **Multi-Factor Authentication (MFA)** and offer **Single Sign-On (SSO)** for secure login  
- Review and harden authentication and access control policies

---

## 📎 Supporting Document

- [📄 PASTA_worksheet.pdf](PASTA_worksheet.pdf)

This PDF includes the full breakdown across the 7 stages of the PASTA threat modeling framework.

---

> 🗒️ *This project is based on a fictional security scenario and used for educational purposes.*
