---
Status: ⚠️ Draft
---

# What is due diligence?

Under the Cyber Resilience Act, _due diligence_ refers to the obligation of [manufacturers][] to ensure that any third-party components integrated into their products, including Free and Open Source Software, adhere to the essential cybersecurity requirements of [[Annex I]]. Manufacturers remain responsible for the security of the final [product][] as a whole, and failure to comply may result in administrative [fines][]. 

The appropriate level of _due diligence_ depends on the nature and cybersecurity risk of the component. As outlined in [[Recital 34]], _due diligence_ typically involves one or more of the following actions:

* **Verifying conformity:** Checking if the component already bears the [CE marking][] or has demonstrated conformity with the CRA, for example through a [security attestation][].
* **Checking maintenance:** Verifying that the component receives regular security updates (e.g., checking its update history).
* **Vulnerability scanning:** Ensuring the component is free from known vulnerabilities listed in public databases (e.g., the ENISA database).
* **Security testing:** Carrying out additional security tests relative to the risk.

If a vulnerability is identified during this process, the manufacturer must remediate it and share the applied fix with the upstream maintainer (i.e., open a merge/pull request upstream).

[manufacturers]: ../manufacturers/what-is-a-manufacturer.md
[product]: ../cra-itself/scope.md
[fines]: ../manufacturers/mistakes.md
[CE marking]: ../cra-itself/ce-mark.md
[security attestation]: ../attestations/what-is-a-security-attestation.md
