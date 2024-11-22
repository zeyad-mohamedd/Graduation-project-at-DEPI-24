# Mobile Application Penetration Testing

## Digital Egypt Pioneers Initiative (DEPI)
- **Instructor:** Mamdouh El-Tahiry  
- **Company:** Next Academy  
- **Group Code:** DKH1_lSS5_S1e  

---

## Prepared By:
- Abdelrahman Gomah Mohamed Swidan  
- Mohamed Adel AbuZaid Ismail  
- Ziad Mohamed Abd El-Hamid Mohamed  
- Mohamed Makram Mohamed El Shaboury  
- Noor Mahmoud Mohamed Mohasseb  

---

## Project Details:
- **Title:** Mobile Application Penetration Testing  
- **Project Duration:** 1/10/2024 - 20/10/2024  
- **SHA1:** 19b741c1ac9a48eb7366bfce3f7eb496af09704e  

---

## Table of Contents:
1. [Executive Summary](#executive-summary)  
2. [Scope of Report](#scope-of-report)  
3. [Compliance Framework Used](#compliance-framework-used)  
4. [Vulnerability Checklist](#vulnerability-checklist)  
5. [Assessment Methodology](#assessment-methodology)  
6. [Key Vulnerabilities](#key-vulnerabilities)  
7. [Tools](#tools)  
8. [Conclusion](#conclusion)  

---

## Executive Summary:
This penetration testing report analyzes the security vulnerabilities in a mobile application, emphasizing critical risks to user data and app integrity. The assessment combined automated tools and manual testing techniques. Key vulnerabilities include emulator detection bypass, weak authentication, insecure data storage, and Firebase misconfigurations.

---

## Scope of Report:
- **Target Application:** Triple S Mobile Application v1  
- **Backend Service:** Triple S mobile backend APIs and infrastructure  

---

## Compliance Framework Used:
- **OWASP Mobile Top 10:** Industry-standard framework for mobile application risks.  
- **MASVS (Mobile Application Security Verification Standard):** A detailed standard for resilience, secure storage, and authentication mechanisms.

---

## Vulnerability Checklist:
| No. | Vulnerability Name                                          | Severity  | Status |
|-----|------------------------------------------------------------|-----------|--------|
| 1   | MASVS-RESILIENCE-1: Emulator, Root, and Debugging Detection | Medium    | Found  |
| 2   | MASVS-RESILIENCE-2: Vulnerability to Janus (CVE-2017-13156) | High      | Found  |
| 3   | MASVS-RESILIENCE-3: Obfuscation                             | Medium    | Found  |
| 4   | Insecure Data Storage                                       | High      | Found  |
| 5   | Insecure Authentication Mechanism                          | Critical  | Found  |
| 6   | Insecure OTP Handling in `updateMe` API                     | High      | Found  |
| 7   | Lack of Rate Limiting & Weak OTP Mechanism                  | High      | Found  |
| 8   | Weak Authentication Mechanism                               | High      | Found  |
| 9   | Firebase Misconfiguration                                   | High      | Found  |
| 10  | Insecure Direct Object Reference (IDOR)                    | High      | Found  |

---

## Assessment Methodology:
1. **Preparation:** Define scope and objectives.  
2. **Static Analysis:** Analyze the code for flaws and vulnerabilities.  
3. **Dynamic Analysis:** Evaluate app behavior during runtime.  
4. **OWASP MASVS Testing:** Ensure compliance with security standards.  
5. **Backend Services Testing:** Test APIs and backend services for vulnerabilities.  
6. **Reporting:** Document findings and recommendations.  
7. **Follow-up:** Verify fixes and reassess vulnerabilities.

---

## Key Vulnerabilities:
1. **Emulator, Root, and Debugging Detection Bypassed:**  
   - Severity: Medium  
   - Description: Protections against rooted devices and emulators can be bypassed using Frida scripts.  
   - Recommendation: Implement robust detection mechanisms.

2. **Insecure Data Storage:**  
   - Severity: High  
   - Description: Sensitive data stored in shared preferences and cache is vulnerable to unauthorized access.  
   - Recommendation: Encrypt all sensitive data and use secure storage methods.

3. **Weak Authentication Mechanism:**  
   - Severity: Critical  
   - Description: Registration requests bypass email confirmation and admin approval.  
   - Recommendation: Enforce strict validation and multi-factor authentication.

4. **Firebase Misconfiguration:**  
   - Severity: High  
   - Description: Unrestricted file uploads and public access to sensitive data.  
   - Recommendation: Enforce Firebase security rules and restrict public access.

(For a full list of vulnerabilities, see the [Vulnerability Checklist](#vulnerability-checklist).)

---

## Tools:
- **MobSF:** Automated vulnerability analysis.  
- **Frida:** Dynamic instrumentation toolkit.  
- **Burp Suite:** Web vulnerability scanner.  
- **APKTool:** Reverse engineering APKs.  
- **ADB Tools:** Android debugging tools.  
- **FFUF:** Brute force testing tool.  

---

## Conclusion:
The assessment identified critical security flaws in the mobile application, posing risks such as unauthorized access and data breaches. Implementing the recommendations in this report will significantly enhance the app's security. Regular updates and testing are crucial to maintaining long-term protection.
