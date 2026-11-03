---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/305
---

# What level of due diligence is reasonable for manufacturers integrating open source components?

The reasonable level of due diligence for an open source component depends on the nature and level of cybersecurity risk of that component, as for any other third-party component. The Commission's FAQ says so: _"the appropriate level of due diligence is dependent on the nature and level of cybersecurity risk of a given open-source component"_ ([[official/faq_4-4-4]], [[official/faq_4-4-2]]). You may integrate open source components outside the scope of the CRA, or published by an open-source software steward, as long as they do not compromise the cybersecurity of your product ([[official/faq_4-4-4]], [[CRA Article 13(5)]]).

[[CRA Recital 34]] lists the actions to choose from, one or more depending on the risk ([[official/faq_4-4-2]]):

- checking whether the component bears the CE marking or has otherwise demonstrated conformity with the CRA; most open source components will not, which is allowed ([[official/faq_4-4-3]]);
- verifying that it receives regular security updates, for example from its security update history;
- checking that it is free from vulnerabilities registered in the European vulnerability database or other public databases;
- carrying out additional security tests where appropriate.

The Commission's FAQ adds examples such as software composition analysis, reviewing the component's SBOM and checking its support period ([[official/faq_4-4-2]]); the Commission's guidance puts it as working out what your product needs from the component and verifying that it delivers it ([[CRA-GUIDANCE point 171]]).

If you find a vulnerability in the component, you have to report it to whoever maintains it, fix it in your product, and share any fix you develop with them ([[CRA Article 13(6)]], [[CRA-GUIDANCE Section 9.2.1]]).

The CRA also lets the Commission set up voluntary security attestation programmes for open source software, which the Commission's FAQ says _"would facilitate manufacturers' due diligence obligation"_ where available ([[CRA Article 25]], [[official/faq_4-4-4]]). See [[due-diligence/what-is-due-diligence]] for the obligation in general and [[due-diligence/relation-to-attestations]] for attestations.
