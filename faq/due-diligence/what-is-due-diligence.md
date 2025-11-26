---
Status: ⚠️ Draft
---

# What is due diligence?

Under the Cyber Resilience Act, **due diligence** refers to the obligation of manufacturers to ensure that any third-party components integrated into their products, including Free and Open Source Software, adhere to essential cybersecurity requirements. [Manufacturers](https://cra.orcwg.org/faq/manufacturers/what-is-a-manufacturer/) remain responsible for the security of the final [product](https://cra.orcwg.org/faq/cra-itself/scope/) as a whole, and failure to comply may result in administrative [fines](https://cra.orcwg.org/faq/manufacturers/mistakes/). 

The appropriate level of due diligence depends on the nature and cybersecurity risk of the component. 
As outlined in [Recital 34](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_34), typically, it involves one or more of the following actions:

* **Verifying conformity:** Checking if the component already bears the CE marking or has demonstrated conformity with the CRA.
* **Checking maintenance:** Verifying that the component receives regular security updates (e.g., checking its update history).
* **Vulnerability scanning:** Ensuring the component is free from known vulnerabilities listed in public databases (e.g., the ENISA database).
* **Security testing:** Carrying out additional security tests relative to the risk.

If a vulnerability is identified during this process, the manufacturer must remediate it and share the applied fix with the upstream maintainer (i.e., open a merge/pull request upstream).
