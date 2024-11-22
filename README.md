# 🔒💻 **Mobile Application Penetration Testing** 👨‍💻


## 🎓 **Digital Egypt Pioneers Initiative (DEPI)**  
- **👨‍🏫 Instructor:** Mamdouh El-Tahiry  
- **🏢 Company:** Next Academy  
- **🆔 Group Code:** `DKH1_lSS5_S1e`  

---

## 👥 **Prepared By:**  
- 💼 Abdelrahman Gomah Mohamed Swidan  
- 💼 Mohamed Adel AbuZaid Ismail  
- 💼 Ziad Mohamed Abd El-Hamid Mohamed  
- 💼 Mohamed Makram Mohamed El Shaboury  
- 💼 Noor Mahmoud Mohamed Mohasseb  

---

## 📅 **Project Details:**  
- **📋 Title:** Mobile Application Penetration Testing  
- **⏳ Project Duration:** `1/10/2024 - 20/10/2024`  
- **🔑 SHA1:** `19b741c1ac9a48eb7366bfce3f7eb496af09704e`  

---

## 📜 **Table of Contents:**  
1. [✨ Executive Summary](#-executive-summary)  
2. [🛡️ Scope of Report](#-scope-of-report)  
3. [📚 Compliance Framework Used](#-compliance-framework-used)  
4. [⚠️ Vulnerability Checklist](#-vulnerability-checklist)  
5. [🛠️ Assessment Methodology](#-assessment-methodology)  
6. [🐞 Key Vulnerabilities](#-key-vulnerabilities)  
7. [🔧 Tools](#-tools)  
8. [📌 Conclusion](#-conclusion)  

---

## ✨ **Executive Summary:**  
This penetration testing report identifies critical vulnerabilities in the mobile application that could compromise user data and application integrity. The analysis included **automated tools** and **manual techniques**, with notable findings such as:  
- **⚙️ Weak Authentication Mechanism**  
- **📂 Insecure Data Storage**  
- **🛠️ Emulator Detection Bypassing**  
- **📁 Firebase Misconfiguration**

---

## 🛡️ **Scope of Report:**  
- **🎯 Target Application:** Triple S Mobile Application v1  
- **🔗 Backend Service:** Triple S mobile backend APIs and infrastructure  

---

## 📚 **Compliance Framework Used:**  
- **📊 OWASP Mobile Top 10:** A global standard for securing mobile applications.  
- **📜 MASVS (Mobile Application Security Verification Standard):** Focused on resilience, secure storage, and authentication.

---

## ⚠️ **Vulnerability Checklist:**  
| 🆔 No. | 🐞 Vulnerability Name                                      | 🔥 Severity  | ✅ Status |
|-------|----------------------------------------------------------|-------------|----------|
| 1️⃣   | MASVS-RESILIENCE-1: Emulator, Root, and Debugging Detection | 🟠 Medium    | ✅ Found  |
| 2️⃣   | MASVS-RESILIENCE-2: Vulnerability to Janus (CVE-2017-13156) | 🔴 High      | ✅ Found  |
| 3️⃣   | MASVS-RESILIENCE-3: Obfuscation                             | 🟢 Medium    | ✅ Found  |
| 4️⃣   | Insecure Data Storage                                       | 🔴 High      | ✅ Found  |
| 5️⃣   | Insecure Authentication Mechanism                          | 🔥 Critical  | ✅ Found  |
| 6️⃣   | Insecure OTP Handling in `updateMe` API                     | 🔴 High      | ✅ Found  |
| 7️⃣   | Lack of Rate Limiting & Weak OTP Mechanism                  | 🔴 High      | ✅ Found  |
| 8️⃣   | Weak Authentication Mechanism                               | 🔴 High      | ✅ Found  |
| 9️⃣   | Firebase Misconfiguration                                   | 🔴 High      | ✅ Found  |
| 🔟   | Insecure Direct Object Reference (IDOR)                    | 🔴 High      | ✅ Found  |

---

## 🛠️ **Assessment Methodology:**  
1. **📝 Preparation:** Defined scope and objectives.  
2. **🔍 Static Analysis:** Analyzed code for flaws.  
3. **⚡ Dynamic Analysis:** Tested app behavior in runtime.  
4. **📑 OWASP MASVS Testing:** Ensured compliance with security standards.  
5. **🔐 Backend Services Testing:** Examined APIs for vulnerabilities.  
6. **🖋️ Reporting:** Documented findings and recommendations.  
7. **🔄 Follow-up:** Verified fixes and reassessed vulnerabilities.  

---

## 🐞 **Key Vulnerabilities:**  
### ⚙️ **1. Emulator, Root, and Debugging Detection Bypassed**  
- **Severity:** 🟠 Medium  
- **Impact:** Attackers can reverse engineer or modify the app.  
- **Recommendation:** Enhance emulator/root detection mechanisms.

### 📂 **2. Insecure Data Storage**  
- **Severity:** 🔴 High  
- **Impact:** Sensitive data stored in shared preferences can be accessed by attackers.  
- **Recommendation:** Encrypt all sensitive data and use secure storage mechanisms.

### 🔒 **3. Weak Authentication Mechanism**  
- **Severity:** 🔥 Critical  
- **Impact:** Registration requests bypass validation, enabling unauthorized access.  
- **Recommendation:** Enforce strict validation and implement multi-factor authentication.

### 📁 **4. Firebase Misconfiguration**  
- **Severity:** 🔴 High  
- **Impact:** Public access allows uploading arbitrary files and accessing sensitive data.  
- **Recommendation:** Restrict public access and enforce Firebase security rules.

_For a detailed list, refer to the [Vulnerability Checklist](#-vulnerability-checklist)._  

---

## 🔧 **Tools:**  
- 🔍 **MobSF:** Automated vulnerability analysis.  
- 🔧 **Frida:** Dynamic instrumentation toolkit.  
- 🛠️ **Burp Suite:** Web vulnerability scanner.  
- 📂 **APKTool:** Reverse engineering APKs.  
- 💻 **ADB Tools:** Debugging Android apps.  
- 🛡️ **FFUF:** Brute force testing tool.  

---

## 📌 **Conclusion:**  
This penetration testing project highlights critical vulnerabilities that need immediate remediation to enhance application security. Key recommendations include:  
- **✅ Implementing strict access controls.**  
- **✅ Encrypting sensitive data.**  
- **✅ Regular security audits.**

🔒 By addressing these issues, the app can better protect user data and maintain long-term security.  
**📢 Regular testing and updates are crucial to keeping the app resilient against evolving threats!**
