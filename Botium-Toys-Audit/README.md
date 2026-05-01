# Internal Security Audit: Botium Toys 🧸🔒

## 📝 Project Overview
This project consists of an internal security audit for **Botium Toys**, a small but growing toy company that has expanded its market internationally (U.S. and E.U.). 

As an entry-level security analyst, my goal was to assess the current security posture of the organization, identify risks, and ensure compliance with global regulations such as **GDPR** and **PCI DSS**.

## 🎯 Audit Goals & Scope
*   **Scope:** The entire security program at Botium Toys, including physical and digital assets, internal processes, and data management.
*   **Goals:** 
    *   Assess existing assets against the **NIST Cybersecurity Framework (CSF)**.
    *   Identify gaps in technical, administrative, and physical controls.
    *   Ensure adherence to international compliance standards for online payments and data privacy.

## 🔍 Key Findings & Risk Assessment
The organization currently has a **Risk Score of 8/10**, indicating a high-risk posture due to missing critical controls.

### 🛡️ Existing Controls (What is working)
*   **Physical Security:** Sufficient locks, up-to-date CCTV surveillance, and fire detection systems are in place.
*   **Network Defense:** An active firewall is configured with defined security rules.
*   **Endpoint Protection:** Antivirus software is installed and monitored regularly.

### ⚠️ Identified Gaps (Critical Risks)
*   **Data Protection:** No encryption is used for credit card data (local storage/transmission), failing **PCI DSS** standards.
*   **Access Management:** Failure to implement the **Principle of Least Privilege** and **Separation of Duties**; all employees have access to sensitive data.
*   **Resilience:** Absence of a **Disaster Recovery Plan** and regular data backups.
*   **Detection:** No **Intrusion Detection System (IDS)** has been installed.

## 📜 Compliance Evaluation
*   **PCI DSS:** Non-compliant due to lack of encryption and improper access to cardholder data.
*   **GDPR:** Partially compliant; breach notification plans exist, but data classification and inventorying are missing.
*   **SOC Type 1 & 2:** Non-compliant due to the absence of established user access policies and lack of confidentiality for PII/SPII].

## 💡 Recommendations
1.  **High Priority:** Implement **AES-256 encryption** for all customer financial data to meet PCI DSS requirements].
2.  **Access Control:** Apply **Least Privilege** policies immediately, ensuring employees only access data necessary for their roles].
3.  **Business Continuity:** Establish a centralized **Backup and Disaster Recovery Strategy** to ensure data availability in case of a breach or system failure.
4.  **Network Monitoring:** Deploy an **IDS** to detect and alert on anomalous traffic.

---
*This project was completed as part of the Google Cybersecurity Professional Certificate.*
