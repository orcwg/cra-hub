---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/305
---

# What is due diligence?

Under the CRA, _due diligence_ is what a manufacturer has to do when it builds components made by others into its product: make sure those components do not compromise the cybersecurity of the product ([[CRA Article 13(5)]]). The Commission's FAQ says manufacturers can integrate components of all kinds, including open source components outside the CRA's scope, _"but they must ensure that such components do not compromise the cybersecurity of their products with digital elements"_ ([[official/faq_4-4-1]]). The components themselves do not have to meet the essential cybersecurity requirements of [[CRA Annex I]]; the product as a whole does ([[official/faq_4-4-3]]).

The Commission's guidance describes due diligence as _"determining what the product with digital elements requires from its components in order to meet its cybersecurity objectives, and verifying, in a risk-based manner, that those components are in line with the product's needs"_ ([[CRA-GUIDANCE point 170]]). If the product relies on a component for cryptography, updates or secure communications, the manufacturer checks that the component delivers them, from its documentation and, where needed, its own tests ([[CRA-GUIDANCE point 171]]).

How much checking that takes depends on the component's risk ([[official/faq_4-4-2]]). [[CRA Recital 34]] and the Commission's FAQ list the actions to choose from:

- checking whether the component bears the CE marking or has otherwise shown conformity with the CRA;
- checking that it receives regular security updates;
- checking public vulnerability databases for vulnerabilities that affect it;
- running additional security tests, such as fuzzing or penetration testing;
- reviewing its software bill of materials, support period and intended purpose, and isolating highly critical components ([[official/faq_4-4-2]]).

A vulnerability found in a component has to be reported to whoever maintains it, and any fix shared with them ([[CRA Article 13(6)]]). The manufacturer remains responsible for its product as a whole: see [[manufacturers/mistakes]].

For open source components in particular, see [[due-diligence/foss]]; for the CE marking, see [[cra-itself/ce-mark]].
