---
Status: ⚠️ Draft
Related issues: https://github.com/orcwg/cra-hub/issues/305
---

# What is due diligence?

Under the Cyber Resilience Act, _due diligence_ is what [manufacturers][] have to do when they integrate third-party components, including Free and Open Source Software, into their products. The Commission's FAQ puts it this way: manufacturers can integrate components of all kinds, including open source components outside the scope of the CRA, _"but they must ensure that such components do not compromise the cybersecurity of their products with digital elements"_ ([[official/faq_4-4-1]], [[CRA Article 13(5)]]). Components don't have to meet the essential cybersecurity requirements of [[CRA Annex I]] themselves; the product as a whole does (see [[due-diligence/essential-requirements]]). Manufacturers remain responsible for the security of the final [product][] as a whole, and failure to comply may result in administrative [fines][].

The appropriate level of _due diligence_ depends on the nature and cybersecurity risk of the component ([[official/faq_4-4-2]]). As outlined in [[CRA Recital 34]], _due diligence_ typically involves one or more of the following actions:

* **Verifying conformity:** Checking if the component already bears the [CE marking][] or has demonstrated conformity with the CRA, for example through a [security attestation][].
* **Checking maintenance:** Verifying that the component receives regular security updates (e.g., checking its update history).
* **Vulnerability scanning:** Ensuring the component is free from known vulnerabilities listed in public databases (e.g., the ENISA database).
* **Security testing:** Carrying out additional security tests relative to the risk.

If a vulnerability is identified during this process, the manufacturer must remediate it and share the applied fix with the upstream maintainer (i.e., open a merge/pull request upstream) ([[official/faq_4-3-6]], [[CRA Article 13(6)]]).

The actions above are examples, not a checklist: see [[due-diligence/recital-34]]. For open source components, see [[due-diligence/foss]].

[manufacturers]: ../manufacturers/what-is-a-manufacturer.md
[product]: ../cra-itself/scope.md
[fines]: ../manufacturers/mistakes.md
[CE marking]: ../cra-itself/ce-mark.md
[security attestation]: ../attestations/what-is-a-security-attestation.md
