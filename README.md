# Mock RMF Implementation for DoD Web Application

This repository demonstrates a mock implementation of the NIST Risk Management Framework (RMF) for a fictional Department of Defense web application. It is structured to reflect each of the six RMF steps and includes simulated documents such as system categorization, control selection, STIG compliance, eMASS package visuals, ACAS scan samples, and a POA&M.

## 🔐 Tools and Frameworks Used
- DISA STIG Viewer
- eMASS (mocked screenshots)
- ACAS (simulated Nessus reports)
- NIST SP 800-53 Rev 5
- POA&M Templates
- Excel & Markdown Documentation

## 📊 Purpose
Designed to showcase my understanding of RMF implementation and cybersecurity compliance in a DoD environment, this project is part of my portfolio to demonstrate eligibility for federal ISSO/ISSM roles.

---
# 🛡️ Mock RMF Implementation for a DoD Web Application

This repository contains a mock Risk Management Framework (RMF) implementation for a fictional Department of Defense web-based system. It demonstrates practical knowledge of NIST SP 800-37 and SP 800-53 controls, system categorization, control selection, assessment planning, and POA&M creation.

## 📂 Repository Contents

- **1-Categorization/**: System categorization report based on FIPS 199 and NIST SP 800-60.
- **4-Assessment/**: Sample POA&M with mock findings and mitigation strategies.
- **eMASS-Screenshots/**: Simulated screenshots of an eMASS system entry (to be added).
- **ACAS-Scan-Reports/**: Sample Nessus/ACAS scan findings.

## 🧰 Tools Used

- NIST SP 800-53 Rev. 5
- DISA STIG Viewer
- ACAS/Nessus (mocked reports)
- eMASS (mock simulation)
- Excel, Markdown, PowerShell (for scriptable remediations)

## 🧠 Objective

To showcase understanding of RMF lifecycle processes, FISMA/NIST compliance, STIGs, and control implementation in support of DoD ATO efforts. Suitable for roles in ISSO, ISSM, or Cybersecurity Analyst supporting RMF and DIACAP transitions.

---

# 📄 System Categorization Report

**System Name:** DoD Medical Web Portal (Mock)  
**System Owner:** Defense Health Agency  
**Prepared By:** Kim Matthews  
**Date:** May 2025  

---

## 1. System Description

A fictional web application used to store and retrieve patient health records across DoD clinics. Hosted on-prem within a secure enclave and accessible to internal personnel via CAC authentication.

---

## 2. FIPS 199 Categorization

| Security Objective | Impact Level | Justification |
|--------------------|--------------|---------------|
| Confidentiality    | High         | Medical records are sensitive PII/PHI. Unauthorized access could result in harm to individuals. |
| Integrity          | Moderate     | Accuracy of health data is critical, but errors may be correctable through procedures. |
| Availability       | Moderate     | Temporary system outages would delay access but not endanger life immediately. |

**Overall Impact Level:** HIGH

---

## 3. Boundary Diagram

*(To be uploaded: diagram of enclave, DMZ, database, and user roles)*

---

## 4. Authorizing Official

Name: Jane Doe, SES  
Organization: Defense Health Cybersecurity Operations Center  
Email: jane.doe@dodsoc.mil  

# 📊 Plan of Actions & Milestones (POA&M)

**System:** DoD Medical Web Portal  
**Author:** Kim Matthews  
**Date:** May 2025  

---

| # | Vulnerability Title                   | Risk Level | Date Identified | Remediation Plan                           | Milestone Date | Responsible Party |
|---|--------------------------------------|------------|------------------|--------------------------------------------|----------------|-------------------|
| 1 | Windows Server 2022: SMBv1 Enabled   | High       | 05/10/2025       | Disable SMBv1 via PowerShell               | 05/20/2025     | SysAdmin Team     |
| 2 | Web App: TLS 1.0 Enabled             | Medium     | 05/12/2025       | Update server configuration to disable TLS 1.0/1.1 | 05/25/2025     | DevOps Team       |
| 3 | Incomplete STIG Checklist (Web Tier) | Medium     | 05/14/2025       | Complete manual checklist, verify findings | 05/28/2025     | ISSO              |
| 4 | Audit Logs Not Centralized           | High       | 05/15/2025       | Forward logs to SIEM via Syslog            | 06/01/2025     | Security Team     |

---

## Notes

- All findings were identified via mock ACAS and STIG assessments.
- Risk levels are based on CVSS and DoD risk tolerance guidelines.
- This POA&M will be uploaded to the eMASS package for ATO readiness.
