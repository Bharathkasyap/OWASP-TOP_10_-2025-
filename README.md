
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

## Note:
This document is based on the latest public OWASP project pages as of June 2025. Web Application Top 10 (2025) is pending official release.
