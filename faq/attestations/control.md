---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/306
---

# Can an open source project control who issues security attestations for it?

No, an open source project cannot control who issues security attestations for it: the CRA opens attestations to anyone, not just the project's maintainers or its steward. What a project can control is which attestations it endorses and how its name is used.

Neither the Commission's FAQ nor its guidance says who may issue an attestation or whether a project can limit it; the guidance does not cover attestations at all. What the Commission's FAQ does say is what the programmes are for: the Commission _"is empowered to establish voluntary security attestations programmes that can be used to assess the conformity of free and open-source components with the CRA"_, and where available they _"would facilitate manufacturers' due diligence obligation"_ ([[official/faq_4-4-4]]). The programmes do not exist yet (see [[attestations/what-is-a-security-attestation]]).

On who may issue them, the CRA's text is what there is, and it points one way. Programmes must allow _"the developers or users of products with digital elements qualifying as free and open-source software as well as other third parties"_ to assess a project's conformity ([[CRA Article 25]]), and should be designed so that not only the people developing or contributing to the project can _"initiate or finance a security attestation"_, _"but also third parties, such as manufacturers that integrate such products into their own products with digital elements, users, or Union and national public administrations"_ ([[CRA Recital 21]]). Our reading is that nothing in this gives a project a veto, and that a programme limited to the project or its steward would go against the design the CRA asks for.

That follows from what the Commission's FAQ says attestations are for: they serve the manufacturer's due diligence, not the project. A manufacturer that integrates your software has to make sure it does not compromise its product's security ([[CRA Article 13(5)]]), and the Commission's FAQ lists how: checking the component's security update history, its known vulnerabilities, its SBOM and support period, running its own security tests, and assessing the security posture of whoever produces it ([[official/faq_4-4-2]]); the guidance adds documentation and assurance evidence from the component's producer ([[CRA-GUIDANCE point 171]]). An attestation is one more piece of evidence for that assessment. Since a manufacturer can always assess your software itself or have someone do it, restricting who may issue an attestation would not restrict who may assess the software.

That leaves you three practical levers:

- **Choose which attestations you promote.** Nothing stops you from linking to the attestations you took part in, or vetted, and ignoring the rest. Downstream users and manufacturers will treat the ones your project stands behind as the reference.
- **Protect your name.** An attestation can describe your software; it cannot use your project's trademark to suggest you endorsed it without your permission. That protection comes from trademark law, not from the CRA, so it only helps if your project or its steward holds the trademark.
- **Make the project's own attestation the better one.** Manufacturers have to weigh the evidence they rely on ([[CRA-GUIDANCE point 171]]). Maintainers and stewards know the codebase and its development and security processes, and can commit to fixing what an assessment finds; an outside assessor working without the project's cooperation has less information and no such commitment. That gives attestations issued or vetted by the project an edge, and is a reason for projects, stewards and third-party assessors to work together rather than compete.

The Commission may clarify how these programmes work, including who can issue attestations under them, in the delegated acts that create them ([[CRA Article 25]], [[CRA Recital 117]]).

For what due diligence on open source components looks like in practice, see [[due-diligence/foss]].
