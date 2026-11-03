---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/305
---

# Do open source components have to meet the essential requirements of Annex I before I integrate them?

No, you don't have to bring an open source component, or any other third-party component, into compliance with the essential cybersecurity requirements of Annex I before integrating it. The Commission's FAQ says so in terms: _"The manufacturer does not need to bring such components into compliance with the essential requirements set out in Annex I, part I, before integrating them"_ ([[official/faq_4-4-3]]). What you have to make sure of is that your product as a whole meets them, and that the component does not compromise its security ([[CRA Article 13(5)]], [[CRA-GUIDANCE point 173]]).

The Commission's guidance draws the same line: where you develop functionality yourself, you implement the essential requirements directly; where you integrate components developed by others, you ensure through due diligence _"that those components can be used in a way that enables the product with digital elements as a whole to comply"_ ([[CRA-GUIDANCE point 173]]). So the question to ask of a component is not whether it would pass Annex I on its own, but what your product needs from it and whether it delivers that ([[CRA-GUIDANCE point 170]], [[CRA-GUIDANCE point 171]]). Where a component falls short of what your product needs, you address that in the product: by configuring or isolating the component, adding product-level measures, or switching to another one ([[official/faq_4-4-2]], [[official/faq_4-3-6]]). How much checking that takes is covered in [[due-diligence/recital-34]] and, for open source components, [[due-diligence/foss]].

Security attestations are not a bar a component has to clear either. The Commission's FAQ says that the voluntary attestation programmes the CRA lets the Commission set up for open source software _"would facilitate manufacturers' due diligence obligation"_ where available ([[official/faq_4-4-4]], [[CRA Article 25]]): an attestation is evidence you can rely on in your due diligence, of the kind the guidance calls _"conformity or assurance documentation"_ ([[CRA-GUIDANCE point 171]]). No such programme exists yet: see [[attestations/what-is-a-security-attestation]].

One part of Annex I does reach integrated components, through you. The Commission's FAQ adds that you also have to _"comply with the vulnerability handling obligations of Annex I, Part II, for the duration of the support period, for their products in their entirety"_ ([[official/faq_4-4-3]], [[CRA Annex I, Part II]]). A vulnerability in an open source component is yours to handle in your product, and to report and share upstream ([[official/faq_4-3-6]], [[CRA Article 13(6)]]).
