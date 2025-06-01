
# OWASP Top 10 – 2025 Overview (Unofficial Summary as of June 2025)

As of June 2025, OWASP has not yet officially released the updated Top 10 for Web Applications. The latest official version remains the **OWASP Top 10 – 2021**. However, several newer OWASP Top 10 lists have been released for specialized areas, including Large Language Models (LLMs), Non-Human Identities (NHIs), and Smart Contracts.

---

## 🔐 OWASP Top 10 for Large Language Model (LLM) Applications (2025)

1. **Prompt Injection**  
   Attackers manipulate input prompts to trick LLMs into producing harmful or unauthorized outputs.

2. **Insecure Output Handling**  
   LLM responses are used without validation, leading to injection or execution risks.

3. **Training Data Poisoning**  
   Malicious data is fed during training, affecting model behavior and causing trust issues.

4. **Model Denial of Service (DoS)**  
   High resource-consuming prompts can exhaust system memory or processing.

5. **Supply Chain Vulnerabilities**  
   Third-party models or data can introduce backdoors and weak links.

6. **Sensitive Information Disclosure**  
   LLMs trained on sensitive data may leak it via responses.

7. **Insecure Plugin Design**  
   Poor validation in LLM plugins can lead to code execution or data leakage.

8. **Excessive Agency**  
   Over-trusting LLMs with autonomous actions without verification can cause damage.

9. **Overreliance**  
   Sole dependence on LLMs leads to unverified or biased decisions.

10. **Model Theft**  
    LLMs and their weights can be stolen if not properly protected.

More: [OWASP LLM Top 10](https://owasp.org/www-project-top-10-for-large-language-model-applications/)

---

## 🤖 OWASP Non-Human Identity (NHI) Top 10 (2025)

1. **Improper Offboarding**  
   Not revoking access of unused NHIs leaves systems open.

2. **Secret Leakage**  
   Exposure of API keys, tokens due to poor storage or logging.

3. **Vulnerable Third-Party NHI**  
   Weak third-party identities add risk.

4. **Insecure Authentication**  
   Poor or missing auth mechanisms for machine identities.

5. **Overprivileged NHI**  
   Granting more permissions than necessary to machine accounts.

6. **Insecure Cloud Deployment Configurations**  
   Misconfigured cloud setups expose NHIs to abuse.

7. **Long-Lived Secrets**  
   Static credentials with no rotation increase attack surface.

8. **Environment Isolation**  
   Lack of boundary separation between prod/dev environments.

9. **NHI Reuse**  
   Using the same identity across systems spreads compromise.

10. **Human Use of NHI**  
    Humans using machine credentials confuses audit trails and increases risk.

More: [OWASP NHI Top 10](https://owasp.org/www-project-non-human-identities-top-10/2025/top-10-2025/)

---

## 💸 OWASP Smart Contract Top 10 (2025)

1. **Access Control Vulnerabilities**  
   Inadequate permission enforcement allows unauthorized function calls.

2. **Price Oracle Manipulation**  
   Attackers feed false data via oracle to influence outcomes.

3. **Logic Errors**  
   Bugs in business logic lead to unintended fund transfers.

4. **Lack of Input Validation**  
   Invalid inputs cause denial-of-service or incorrect execution.

5. **Reentrancy Attacks**  
   Repeated calls before the first completes can drain funds.

6. **Unchecked External Calls**  
   Contracts calling other contracts without checks invite attack vectors.

7. **Flash Loan Attacks**  
   Temporary large loans used to manipulate the contract state.

8. **Integer Overflow/Underflow**  
   Arithmetic calculations exceed or fall below variable limits.

9. **Insecure Randomness**  
   Predictable randomness allows game or lottery manipulation.

10. **Denial of Service (DoS)**  
    Gas limits or blocking functions make contracts unusable.

More: [OWASP Smart Contract Top 10](https://owasp.org/www-project-smart-contract-top-10/)

---

## 🛡️📊🔟 OWASP Top 10 – Comparison: 2021 vs 2025 (Evolving Web Application Security)

The OWASP Top 10 is a globally recognized standard that highlights the most critical security risks to web applications. While the **2021 version** focused on traditional web security threats and application flaws, the upcoming **2025 version** is expected to reflect the shift towards **cloud-native development, AI/ML security**, and **modern software supply chain vulnerabilities**.

---

## 📘 OWASP Top 10 – 2021 Summary

The OWASP Top 10 (2021) emphasized long-standing and well-known issues like injection flaws, access control, misconfigurations, and outdated components. It introduced new categories like **Insecure Design** to capture architectural flaws and **Software and Data Integrity Failures** to reflect risks like dependency confusion and CI/CD pipeline abuse.

Top Highlights:
- A01: Broken Access Control – dominated breach reports
- A03: Injection – included SQLi, XSS, and template injections
- A05: Security Misconfiguration – emphasized lack of secure defaults
- A08: Software and Data Integrity Failures – added due to real-world attacks like SolarWinds

The 2021 list reflected a balanced view between code-level and design-level risks.

---

## 🚀 OWASP Top 10 – 2025 (Expected Trends)

The OWASP Top 10 (2025) is projected to respond to the growing complexity of modern software. Cloud-native architectures, LLM-powered apps, and decentralized components (e.g., APIs, microservices) introduce risks not traditionally captured in older lists.

Expected Enhancements:
- Focus on **LLM Prompt Injection** and **model integrity**
- API-specific issues such as **broken object-level authorization**
- Cloud-focused misconfigurations (e.g., open buckets, insecure IAM)
- Greater emphasis on **SBOM** and third-party dependency risks
- Deprecation or merger of declining issues like SSRF

The 2025 update will shift from just preventing developer mistakes to building **resilience into complex, integrated systems**.

---


# 🔄 OWASP Top 10 – What Changed from 2021 to 2025

| 🔢 2021 Category                        | ⏩ 2025 Direction/Change                                                             | 📝 Key Update Summary                                                                 |
|----------------------------------------|-------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------|
| A01: Broken Access Control             | Expanded to cover API access, Cloud IAM, and zero trust policies                   | More focus on object-level authorization, IAM role abuse in cloud/API environments     |
| A02: Cryptographic Failures            | Emphasizes key rotation, token handling, JWT misconfigurations                     | Shift from weak encryption to real-world crypto management and secret hygiene          |
| A03: Injection                         | Expanded to LLM Prompt Injection, NoSQL, GraphQL                                   | Moves beyond SQLi/XSS to modern, AI and API-based injection risks                      |
| A04: Insecure Design                   | Includes insecure AI model pipelines and LLM architecture flaws                    | Broader scope covering architectural risks in AI and ML systems                        |
| A05: Security Misconfiguration         | Adds IaC (Terraform), K8s misconfig, cloud-native defaults                         | Emphasizes cloud and DevOps stack misconfigurations                                    |
| A06: Vulnerable Components             | Adds Software Bill of Materials (SBOM), open-source risks                          | Includes supply chain attacks and vulnerable AI libraries                              |
| A07: Identification & Auth Failures   | Now includes SSO misconfig, MFA bypass, OAuth/OpenID weaknesses                    | Password handling declines; token and federated auth misuses take lead                 |
| A08: Software & Data Integrity Failure| Covers CI/CD poisoning, LLM training data poisoning                                | Now includes data poisoning in AI and integrity issues in software pipelines           |
| A09: Logging & Monitoring Failures    | Evolved into detection engineering and SIEM integration gaps                       | From basic logging to effective incident detection in hybrid/cloud environments        |
| A10: SSRF                              | Likely deprecated or merged                                                        | Decreased prevalence due to secure-by-default frameworks                               |
---

## 🔄 OWASP Top 10 – 2021 vs 2025: Side-by-Side Comparison

| OWASP 2021                              | OWASP 2025 (Expected Direction)                                                | Key Differences                                                                 |
|----------------------------------------|--------------------------------------------------------------------------------|----------------------------------------------------------------------------------|
| A01: Broken Access Control             | Expanded to include API/Cloud IAM abuses                                      | Extends to multi-cloud & API gateway issues                                      |
| A02: Cryptographic Failures            | Token management, key rotation, encryption hygiene                            | Includes zero-trust token abuse and poor JWT handling                           |
| A03: Injection                         | Includes LLM prompt injection, GraphQL, and NoSQL injections                  | Broader than SQL/XSS – focus on AI/ML and complex data interfaces               |
| A04: Insecure Design                   | May include insecure AI model usage or flawed ML pipelines                    | Focus on flawed architecture involving automation and intelligent systems        |
| A05: Security Misconfiguration         | Cloud-native, K8s, serverless and IaC errors                                  | Now focuses on secure cloud configurations, IaC scanning                        |
| A06: Vulnerable Components             | Includes SBOM, vulnerable AI libraries, and dependency chains                 | Emphasizes integrity of third-party and AI/ML dependencies                      |
| A07: Auth Failures                     | OAuth, OpenID, and misconfigured passwordless auth                            | Passwords take backseat; now it's about SSO, MFA bypass, and misused tokens     |
| A08: Integrity Failures                | LLM training poisoning, unsigned models, CI/CD poisoning                      | Training data and AI model poisoning now under scrutiny                         |
| A09: Logging/Monitoring Failures       | Detection engineering, log centralization, SIEM blind spots                   | Focus shifts to detection capabilities in hybrid environments                   |
| A10: SSRF                              | Possibly merged or dropped                                                    | Fewer SSRF incidents due to improved frameworks and proxy controls              |

---

## 🔍 What This Means for Developers and Security Teams

- **2021** was about fixing known issues in code and infrastructure.
- **2025** is about *anticipating emerging attack vectors* in AI-driven, cloud-based, and decentralized systems.
- Developers must now secure *not just their app logic*, but also pipelines, plugins, models, APIs, and cloud resources.
- Security teams need to focus more on **threat modeling**, **automated detection**, and **supply chain verification**.

---

## 📎 Resources

- [OWASP Top Ten (2021)](https://owasp.org/Top10/)
- [OWASP Project – LLM Top 10](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- [OWASP NHI Top 10 (2025)](https://owasp.org/www-project-non-human-identities-top-10/2025/top-10-2025/)
- [OWASP Smart Contract Top 10](https://owasp.org/www-project-smart-contract-top-10/)

---

Stay tuned and watch the [OWASP Official Site](https://owasp.org) for the full 2025 release. Update your threat models and DevSecOps pipelines accordingly!

## Note:
This document is based on the latest public OWASP project pages as of June 2025. Web Application Top 10 (2025) is pending official release.
