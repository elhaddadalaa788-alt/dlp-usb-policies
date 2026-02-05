 # Data Loss Prevention (DLP) Policies for External Devices

## Overview
This project focuses on designing and implementing **Data Loss Prevention (DLP) policies** to protect sensitive organizational data from leakage through **external devices**, specifically USB storage devices. The project applies the **principle of least privilege** and demonstrates both **policy creation** and **technical enforcement** using a Windows-based environment.

---

## Objectives
- Define and establish DLP security policies to protect confidential information
- Classify organizational data based on sensitivity
- Apply access control and least privilege principles
- Monitor and audit sensitive data usage
- Prevent data leakage through encryption and device control
- Implement and validate USB device restriction policies
- Train users on data security awareness

---

## 1. Introduction to Data Loss Prevention (DLP)

Data Loss Prevention (DLP) refers to a set of security strategies, tools, and policies designed to prevent unauthorized access, disclosure, or exfiltration of sensitive data. DLP is critical in modern organizations due to increasing risks from insider threats, removable media, and human error.

External storage devices such as USB drives pose a high risk because they allow large volumes of data to be copied quickly and removed from secure environments. Implementing strong DLP controls helps ensure data confidentiality, integrity, and compliance with security standards.

---

## 2. Data Classification

TechCo classifies data into the following categories:

### Public Data
- Marketing materials
- Public website content
- Job postings

**Protection Level:** Low  
**Access:** Open to all employees and external users

---

### Internal Data
- Internal emails
- Internal documentation
- Non-sensitive operational data

**Protection Level:** Medium  
**Access:** Employees only

---

### Sensitive Data
- Personally Identifiable Information (PII)
- Financial records
- Customer databases
- Intellectual Property
- Credentials and authentication data

**Protection Level:** High  
**Access:** Restricted to authorized roles only

---

## 3. Access Control and Least Privilege

To enforce least privilege:
- Users are granted **only the minimum access required** to perform their job
- Access permissions are role-based
- Administrative privileges are limited to IT and Security teams
- Permission reviews are conducted periodically

### Permission Review Workflow
1. User requests access
2. Manager approval required
3. IT Security validates necessity
4. Access is logged and audited
5. Periodic review and revocation if no longer required

---

## 4. Monitoring and Auditing

Monitoring and auditing ensure visibility into how sensitive data is accessed and used.

### Tools and Methods
- Windows Event Logs
- Group Policy auditing
- SIEM integration (conceptual)
- DLP alerting rules

### Audited Activities
- USB device connections
- File access attempts
- Policy violations
- Privilege escalation attempts

---

## 5. Leak Prevention Controls

To prevent data leakage, the following controls are applied:

- **USB read/write restrictions**
- **Encryption of sensitive data**
- **Blocking unauthorized removable storage**
- **Policy enforcement via Group Policy**
- **Access logging and alerts**

These controls significantly reduce the risk of accidental or malicious data exfiltration.

---

## 6. Education and Awareness

Employees receive training on:
- Data classification awareness
- Acceptable use of external devices
- Social engineering risks
- Phishing prevention
- Reporting security incidents

Regular security awareness training ensures that users understand their role in protecting sensitive data.

---

## 7. USB Device Restriction Implementation (Windows)

### Environment
- Windows Virtual Machine
- VirtualBox with Extension Pack installed
- USB 2.0 / 3.0 Controller enabled



