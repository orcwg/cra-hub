---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/122, https://github.com/orcwg/cra-hub/issues/67
---

# How can open source projects or their stewards support the due diligence requirements of manufacturers through documentation?

Open source projects and their stewards can support manufacturers' due diligence by voluntarily publishing documentation mirroring a manufacturer's own technical documentation ([[CRA Annex VII]]). This is optional: maintainers of open source software that is not placed on the market _"do not bear obligations in relation to other entities that may integrate such components"_ ([[CRA-GUIDANCE point 87]]), and the only documentation a steward has to produce is its cybersecurity policy ([[CRA Article 24]], [[stewards/documentation]]).

Neither the Commission's FAQ nor its guidance says what a project should publish, but both say what manufacturers check. The Commission's guidance says a manufacturer's evidence may be _"documentation obtained from the component manufacturer, such as technical specifications, security documentation or relevant conformity or assurance documentation"_ ([[CRA-GUIDANCE point 171]]); its FAQ adds the component's update history, SBOM, support period and intended purpose ([[official/faq_4-4-2]]). So, following [[CRA Annex VII]], useful documentation includes:

- **Design and development information**: the software's intended purpose and how its components build on or feed into each other.
- **Vulnerability handling information**: a vulnerability disclosure policy, a contact address for reporting vulnerabilities and how updates are securely distributed, which manufacturers reporting a vulnerability have to follow ([[CRA-GUIDANCE point 223]]).
- **Software bill of materials (SBOM)**: which helps manufacturers understand the supply chain and track vulnerabilities ([[CRA Recital 77]]).

A project that wants to go further can adopt the practices the CRA asks of manufacturers, such as a security policy, an SBOM and a stated support period: see [[projects/practices-to-adopt]]. The due diligence obligation itself stays with the manufacturer ([[CRA Article 13(5)]], [[CRA-GUIDANCE point 88]]); what it involves is covered in [[due-diligence/foss]].

The Commission may also set up voluntary security attestation programmes, which its FAQ says _"would facilitate manufacturers' due diligence obligation"_ ([[official/faq_4-4-4]], [[CRA Article 25]]); as manufacturers and users could finance an attestation ([[CRA Recital 21]]), they could become a source of revenue for a project. None exists yet: see [[attestations/what-is-a-security-attestation]].
