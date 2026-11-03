---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/305
---

# Are the actions listed in Recital 34 a complete list of what due diligence on components requires?

No, the actions listed in Recital 34 are examples of how to exercise due diligence on a third-party component, not a checklist that defines the obligation. What the CRA requires of you is an outcome: the components you integrate, including open source components, must _"not compromise the cybersecurity of the product"_ ([[CRA Article 13(5)]]). How much checking that takes depends on the component and on what your product relies on it for.

Recital 34 itself presents its four actions as things to _"take into account one or more of"_, with the level of due diligence depending on _"the nature and the level of cybersecurity risk associated with a given component"_ ([[CRA Recital 34]]). The four are: checking whether the component's manufacturer has demonstrated conformity with the CRA, for instance through the CE marking; checking that the component receives regular security updates, such as by looking at its security update history; checking that it is free from vulnerabilities registered in the European vulnerability database or other public vulnerability databases; and carrying out additional security tests.

The Commission's FAQ confirms the list is open-ended. It repeats that the more risk a component carries, the more extensive your due diligence should be, and adds examples the recital doesn't name: software composition analysis, sandboxing or isolating highly critical components, reviewing the component's SBOM where it has one, checking its support period, checking that its intended purpose fits the use you make of it, and assessing the security posture of whoever makes it ([[official/faq_4-4-2]]).

The Commission's guidance describes the method behind these examples. Due diligence means _"determining what the product with digital elements requires from its components in order to meet its cybersecurity objectives, and verifying, in a risk-based manner, that those components are in line with the product's needs"_ ([[CRA-GUIDANCE point 170]]). Your product's own risk assessment tells you what you need from each component. If your product relies on a component for cryptography, updates or secure communications, you identify those needs and check that the component meets them, using the component's documentation (technical specifications, security documentation, conformity or assurance documents) and, where appropriate, your own tests ([[CRA-GUIDANCE point 171]]). Which of Recital 34's actions, or others, are the right way to do that follows from what the component does in your product, not from the list.

Due diligence does not mean bringing the component into compliance with Annex I before you use it: see [[due-diligence/essential-requirements]]. For how this applies to open source components specifically, see [[due-diligence/foss]].
