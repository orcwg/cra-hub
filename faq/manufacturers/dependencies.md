---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/97, https://github.com/orcwg/cra-hub/issues/87
---

# Which components and dependencies does a manufacturer have to consider?

All of them that end up in the product, and the remote services the product depends on. A manufacturer's vulnerability handling obligations _"apply to products with digital elements in their entirety, including to all integrated components"_ ([[official/faq_4-3-6]], [[CRA Recital 34]]), its due diligence covers every component sourced from a third party, including open source components never placed on the market ([[CRA Article 13(5)]], [[official/faq_4-4-1]]), and the product includes its _remote data processing solutions_ ([[CRA Article 3(1)]]). The Commission's guidance sums up the cases in a flowchart ([[CRA-GUIDANCE Figure 9]]); in a table:

| What | How the CRA treats it |
|---|---|
| Direct dependencies: the libraries, packages, container images, SDKs and copied-in code your product uses as shipped | A component of the product: due diligence, vulnerability handling, listed in the SBOM ([[CRA Article 13(5)]], [[official/faq_4-3-6]], [[CRA Annex I, Part II]]) |
| Indirect dependencies of an open source component: what it pulls in itself, however many levels down | Yours all the same, since nobody else answers for them: due diligence and vulnerability handling apply; the SBOM only has to list top-level dependencies, which does not shorten your responsibility ([[official/faq_4-3-6]], [[CRA Annex I, Part II]]). A component that is itself a CRA product comes with its manufacturer's declaration, which covers what it contains ([[official/faq_4-4-1]]) |
| Processing at a distance that you designed and developed, or had developed for you, and without which the product cannot perform one of its functions, including software you run on a third party's cloud infrastructure or platform | Part of the product itself: the same requirements and the same conformity assessment ([[CRA Article 3(2)]], [[CRA-GUIDANCE point 184]], [[CRA-GUIDANCE point 198]], [[CRA-GUIDANCE point 199]]; see [[remote-processing/scope]]) |
| A remote service the product needs but you did not develop: a third party's SaaS application, the runtime of its platform, the hypervisor of its infrastructure | Treated like a third-party component: you assess the risks of relying on it, mitigate them in the product, and do due diligence on the provider, for which its own certifications and compliance evidence count ([[CRA-GUIDANCE point 201]], [[CRA-GUIDANCE point 202]], [[CRA-GUIDANCE point 207]]; see [[remote-processing/3rd-party]]) |
| Remote processing the product does not need to function, back-end systems the product never talks to, your own IT and build pipelines | Not part of the product; the risks they pose to it go in your risk assessment ([[CRA-GUIDANCE point 182]], [[CRA-GUIDANCE point 193]], [[CRA-GUIDANCE point 206]]; see [[remote-processing/out-of-scope]]) |

Whether a component came as a library, a package or a copy pasted into your repository does not matter: if it ships, you answer for it. How much checking a component gets depends on its risk, from a CE marking or a security update history to running your own tests ([[official/faq_4-4-2]]; see [[due-diligence/foss]]). A component you have copied in and patched is yours to handle like any other, and the fix you make to it is shared with the project it came from ([[CRA Article 13(6)]]).
