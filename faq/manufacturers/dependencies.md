---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/97, https://github.com/orcwg/cra-hub/issues/87
---

# Which components and dependencies does a manufacturer have to consider?

All of them that end up in the product, and the remote services the product depends on. A manufacturer's vulnerability handling obligations _"apply to products with digital elements in their entirety, including to all integrated components"_ ([[official/faq_4-3-6]], [[CRA Recital 34]]), its due diligence covers every component sourced from a third party, including open source components never placed on the market ([[CRA Article 13(5)]], [[official/faq_4-4-1]]), and the product includes its _remote data processing solutions_ ([[CRA Article 3(1)]]). The Commission's guidance sums up the cases in a flowchart ([[CRA-GUIDANCE Figure 9]]); in a table:

| Dependency | What it covers | Manufacturer's obligations |
|---|---|---|
| In-house component | Software the manufacturer develops itself and builds into the product | Part of the product: the full essential requirements of Annex I, Parts I and II, implemented directly[^1] |
| Direct dependency | Libraries, packages, container images, SDKs and copied-in code used by the product as shipped | A component of the product: due diligence, vulnerability handling, listed in the SBOM[^2] |
| Indirect dependency of an open source component | Software an open source component itself depends on, at any depth. A component that is itself a CRA product is covered by its own manufacturer's declaration[^3] | The same as for a direct dependency: due diligence and vulnerability handling. The SBOM need only list top-level dependencies; responsibility extends to all[^4] |
| Remote data processing solution developed by the manufacturer | Processing at a distance designed and developed by the manufacturer, or under its responsibility, without which the product cannot perform one of its functions, including software run on a third party's cloud infrastructure or platform. The hardware it runs on is not part of the product[^5] | Part of the product: the same essential requirements and conformity assessment. Risks from self-hosted hardware are assessed and mitigated at product level[^6] |
| Third-party remote service | A remote service the product depends on, not developed by the manufacturer: a SaaS application, a platform's runtime, an infrastructure's hypervisor. The provider's own stack is the provider's responsibility, under NIS 2 for cloud providers[^7] | Treated as a third-party component: risk assessment and mitigation in the product, due diligence on the provider, for which the provider's certifications and compliance evidence count[^8] |
| Outside the product | Remote processing not needed for the product's functions, back-end systems the product does not interact with, the manufacturer's own IT and build pipelines[^9] | None as a component; risks to the product are covered by the risk assessment[^10] |

[^1]: [[CRA Article 13(1)]], [[CRA-GUIDANCE point 173]]
[^2]: [[CRA Article 13(5)]], [[official/faq_4-3-6]], [[CRA Annex I, Part II]]
[^3]: [[official/faq_4-4-1]]
[^4]: [[official/faq_4-3-6]], [[CRA Annex I, Part II]]
[^5]: [[CRA Article 3(2)]], [[CRA-GUIDANCE point 180]], [[CRA-GUIDANCE point 184]]; see [[remote-processing/scope]]
[^6]: [[CRA-GUIDANCE point 198]], [[CRA-GUIDANCE point 199]], [[CRA-GUIDANCE point 206]]
[^7]: [[CRA-GUIDANCE point 183]], [[CRA-GUIDANCE point 200]]; see [[remote-processing/3rd-party]]
[^8]: [[CRA-GUIDANCE point 201]], [[CRA-GUIDANCE point 202]], [[CRA-GUIDANCE point 207]]
[^9]: [[CRA-GUIDANCE point 182]], [[CRA-GUIDANCE point 205]]; see [[remote-processing/out-of-scope]]
[^10]: [[CRA-GUIDANCE point 193]], [[CRA-GUIDANCE point 206]]

Whether a component came as a library, a package or a copy pasted into your repository does not matter: if it ships, you answer for it. How much checking a component gets depends on its risk, from a CE marking or a security update history to running your own tests ([[official/faq_4-4-2]]; see [[due-diligence/foss]]). A component you have copied in and patched is yours to handle like any other, and the fix you make to it is shared with the project it came from ([[CRA Article 13(6)]]).
