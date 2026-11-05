---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/97, https://github.com/orcwg/cra-hub/issues/87
---

# Which components and dependencies does a manufacturer have to consider?

All of them that end up in the product, and the remote services the product depends on. A manufacturer's vulnerability handling obligations _"apply to products with digital elements in their entirety, including to all integrated components"_ ([[official/faq_4-3-6]], [[CRA Recital 34]]), its due diligence covers every component sourced from a third party, including open source components never placed on the market ([[CRA Article 13(5)]], [[official/faq_4-4-1]]), and the product includes its _remote data processing solutions_ ([[CRA Article 3(1)]]). The Commission's guidance sums up the cases in a flowchart ([[CRA-GUIDANCE Figure 9]]); in a table:

| Dependency | What it covers | Risk assessment[^1] | Essential requirements[^2] | Due diligence[^3] | Vulnerability handling[^4] |
|---|---|:-:|:-:|:-:|:-:|
| In-house component | Software the manufacturer develops itself and builds into the product[^5] | ✅ | ✅ | N/A | ✅ |
| Direct dependency | Libraries, packages, container images, SDKs and copied-in code used by the product as shipped[^6] | ✅ |  | ✅ | ✅ |
| Vendored component | A component bought from a vendor that placed it on the market under the CRA, with its own declaration of conformity and its own manufacturer handling its vulnerabilities[^7] | ✅ |  | ✅ | ✅, supported by the component manufacturer's |
| Indirect dependency of an open source component | Software an open source component itself depends on, at any depth; the SBOM need only list top-level dependencies[^8] | ✅ |  | ✅ | ✅ |
| Remote data processing solution developed by the manufacturer | Processing at a distance designed and developed by the manufacturer, or under its responsibility, without which the product cannot perform one of its functions, including software run on a third party's cloud; not the hardware it runs on[^9] | ✅, including self-hosted hardware | ✅ | N/A | ✅ |
| Third-party remote service | A remote service the product depends on, not developed by the manufacturer: a SaaS application, a platform's runtime, an infrastructure's hypervisor; the provider's own stack is the provider's responsibility[^10] | ✅ |  | ✅, on the provider | mitigation at product level |
| Outside the product | Remote processing not needed for the product's functions, back-end systems the product does not interact with, the manufacturer's own IT and build pipelines[^11] | ✅ | N/A | N/A | N/A |

[^1]: [[CRA Article 13(2)]], [[CRA Article 13(3)]], [[CRA-GUIDANCE point 167]], [[CRA-GUIDANCE point 206]]
[^2]: [[CRA Article 13(1)]], [[CRA-GUIDANCE point 173]]
[^3]: [[CRA Article 13(5)]], [[official/faq_4-4-1]], [[official/faq_4-4-2]]
[^4]: [[CRA Article 13(8)]], [[CRA Annex I, Part II]], [[official/faq_4-3-6]]
[^5]: [[CRA-GUIDANCE point 173]]
[^6]: [[CRA Recital 34]], [[official/faq_4-3-6]]
[^7]: [[official/faq_4-4-1]], [[official/faq_4-3-6]]
[^8]: [[CRA Annex I, Part II]], [[official/faq_4-3-6]]
[^9]: [[CRA Article 3(2)]], [[CRA-GUIDANCE point 180]], [[CRA-GUIDANCE point 184]], [[CRA-GUIDANCE point 198]], [[CRA-GUIDANCE point 199]]; see [[remote-processing/scope]]
[^10]: [[CRA-GUIDANCE point 183]], [[CRA-GUIDANCE point 200]], [[CRA-GUIDANCE point 201]], [[CRA-GUIDANCE point 202]], [[CRA-GUIDANCE point 207]]; see [[remote-processing/3rd-party]]
[^11]: [[CRA-GUIDANCE point 182]], [[CRA-GUIDANCE point 193]], [[CRA-GUIDANCE point 205]]; see [[remote-processing/out-of-scope]]

Whether a component came as a library, a package or a copy pasted into your repository does not matter: if it ships, you answer for it. How much checking a component gets depends on its risk, from a CE marking or a security update history to running your own tests ([[official/faq_4-4-2]]; see [[due-diligence/foss]]). A component you have copied in and patched is yours to handle like any other, and the fix you make to it is shared with the project it came from ([[CRA Article 13(6)]]).
