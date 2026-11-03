---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/305
---

# What is due diligence?

Under the CRA, _due diligence_ is what a manufacturer has to do when it builds components made by others into its product: make sure those components do not compromise the cybersecurity of the product. [[CRA Article 13(5)]] requires it for every third-party component, _"including when integrating components of free and open-source software that have not been made available on the market in the course of a commercial activity"_. The Commission's FAQ says manufacturers can integrate components of all kinds, including open source components outside the CRA's scope, _"but they must ensure that such components do not compromise the cybersecurity of their products with digital elements"_ ([[official/faq_4-4-1]]). The components themselves do not have to meet the essential cybersecurity requirements of [[CRA Annex I]]; the product as a whole does ([[official/faq_4-4-3]]).

The Commission's guidance describes due diligence as _"determining what the product with digital elements requires from its components in order to meet its cybersecurity objectives, and verifying, in a risk-based manner, that those components are in line with the product's needs"_ ([[CRA-GUIDANCE point 170]]). If the product relies on a component for cryptography, updates or secure communications, the manufacturer identifies those needs and checks that the component meets them, using the component's documentation and, where appropriate, its own tests ([[CRA-GUIDANCE point 171]]).

How much checking that takes depends on the risk: _"the appropriate level of due diligence depends on the nature and level of cybersecurity risk of a given component"_ ([[official/faq_4-4-2]]). The actions [[CRA Recital 34]] lists, and the Commission's FAQ adds to, include:

- checking whether the component already bears the CE marking or has otherwise demonstrated conformity with the CRA;
- verifying that it receives regular security updates, for example from its security update history;
- checking the European vulnerability database and other public databases for vulnerabilities that affect it, and designing the product so that they do not compromise it;
- carrying out additional security tests, such as fuzzing or penetration testing;
- reviewing its software bill of materials, its support period and whether its intended purpose fits the product, and isolating highly critical components ([[official/faq_4-4-2]]).

If the manufacturer finds a vulnerability in the component, it has to report it to whoever maintains the component and, where it develops a fix, share it with them ([[CRA Article 13(6)]]). The manufacturer remains responsible for its product as a whole, and falling short of due diligence is a breach of its own obligations: see [[manufacturers/mistakes]].

For open source components in particular, see [[due-diligence/foss]]; for the CE marking, see [[cra-itself/ce-mark]].
