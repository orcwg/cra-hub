---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/306
---

# Can an open source project control who issues security attestations for it?

No, an open source project cannot control who issues security attestations for it: the CRA deliberately opens attestations to anyone, not just the project's maintainers or its steward. What a project can control is which attestations it endorses and how its name is used.

Security attestation programmes do not exist yet; the Commission may create them to help manufacturers with their due diligence on open source components (see [[attestations/what-is-a-security-attestation]]). When it does, the CRA requires that they allow _"the developers or users of products with digital elements qualifying as free and open-source software as well as other third parties"_ to assess a project's conformity ([[CRA Article 25]]). The recital is explicit that not only the people developing or contributing to the project can _"initiate or finance a security attestation"_, _"but also third parties, such as manufacturers that integrate such products into their own products with digital elements, users, or Union and national public administrations"_ ([[CRA Recital 21]]). Limiting attestations to the project or its steward would go against that design, and nothing in the CRA gives a project a veto. The Commission's guidance does not cover attestations at all.

The reason is that an attestation serves the manufacturer, not the project. A manufacturer that integrates your software has to exercise due diligence on it ([[CRA Article 13(5)]]), and can already do so by checking its update history and known vulnerabilities, by running its own security tests or by relying on documentation and assurance evidence from whoever produced the component ([[CRA Recital 34]], [[CRA-GUIDANCE point 171]], [[official/faq_4-4-2]]). An attestation is one more piece of evidence for that assessment; the Commission's FAQ says attestation programmes, where available, _"would facilitate manufacturers' due diligence obligation"_ ([[official/faq_4-4-4]]). Since a manufacturer can always assess your software itself or have someone do it, restricting who may issue an attestation would not restrict who may assess the software.

That leaves you three practical levers:

- **Choose which attestations you promote.** Nothing stops you from linking to the attestations you took part in, or vetted, and ignoring the rest. Downstream users and manufacturers will treat the ones your project stands behind as the reference.
- **Protect your name.** An attestation can describe your software; it cannot use your project's trademark to suggest you endorsed it without your permission. That protection comes from trademark law, not from the CRA, so it only helps if your project or its steward holds the trademark.
- **Make the project's own attestation the better one.** Manufacturers have to weigh the evidence they rely on ([[CRA-GUIDANCE point 171]]). Maintainers and stewards know the codebase and its development and security processes, and can commit to fixing what an assessment finds; an outside assessor working without the project's cooperation has less information and no such commitment. That gives attestations issued or vetted by the project an edge, and is a reason for projects, stewards and third-party assessors to work together rather than compete.

The Commission may clarify how these programmes work, including who can issue attestations under them, in the delegated acts that create them ([[CRA Article 25]], [[CRA Recital 117]]).

For what due diligence on open source components looks like in practice, see [[due-diligence/foss]].
