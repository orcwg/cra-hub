---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/305
---

# Do open source components have to meet the essential requirements of Annex I before I integrate them?

No, you don't have to bring an open source component, or any other third-party component, into compliance with the essential cybersecurity requirements of Annex I before integrating it. The Commission's FAQ says so directly: _"The manufacturer does not need to bring such components into compliance with the essential requirements set out in Annex I, part I, before integrating them"_ ([[official/faq_4-4-3]]). What you have to ensure is that your product as a whole meets them.

The essential requirements apply to the product you place on the market ([[CRA Article 13(1)]]), and the CRA itself speaks of manufacturers integrating open source components _"that are not subject to the essential cybersecurity requirements"_ ([[CRA Recital 21]]). The Commission's guidance draws the line: where you develop functionality yourself, you implement the essential requirements directly; where you integrate components developed by others, you ensure through due diligence _"that those components can be used in a way that enables the product with digital elements as a whole to comply"_ ([[CRA-GUIDANCE point 173]]). For compliance purposes, integrated third-party components are treated as _"externally supplied components whose properties are verified through due diligence upon integration"_, since you did not design them ([[CRA-GUIDANCE point 172]]).

So the question to ask of a component is not whether it would pass Annex I on its own, but what your product needs from it and whether it delivers that ([[CRA-GUIDANCE point 170]], [[CRA-GUIDANCE point 171]]). Where a component falls short of what your product needs, you address that in the product: by configuring or isolating the component, adding product-level measures, or choosing another one ([[official/faq_4-4-2]]). How much checking that takes is covered in [[due-diligence/recital-34]] and, for open source components, [[due-diligence/foss]].

This is also where security attestations fit. The CRA lets the Commission set up voluntary programmes to assess open source software against _"all or certain essential cybersecurity requirements or other obligations"_ ([[CRA Article 25]]). An attestation would be evidence you can rely on in your due diligence, of the kind the guidance calls _"conformity or assurance documentation"_ ([[CRA-GUIDANCE point 171]], [[official/faq_4-4-4]]); it is not a bar a component has to clear before you can use it, and no such programme exists yet: see [[attestations/what-is-a-security-attestation]].

One part of Annex I does reach integrated components, through you: the vulnerability handling requirements of [[CRA Annex I, Part II]] apply to your product in its entirety, including all integrated components, for the whole support period ([[CRA Recital 34]], [[CRA Article 13(8)]], [[official/faq_4-3-6]]). A vulnerability in an open source component is yours to handle in your product, and to report and share upstream ([[CRA Article 13(6)]]).
