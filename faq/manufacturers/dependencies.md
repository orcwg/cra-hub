---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/97, https://github.com/orcwg/cra-hub/issues/87
---

# Which components and dependencies does a manufacturer have to consider?

All of them that end up in the product. A manufacturer's vulnerability handling obligations _"apply to products with digital elements in their entirety, including to all integrated components"_ ([[official/faq_4-3-6]], [[CRA Recital 34]]), and its due diligence covers every component sourced from a third party, including open source components that were never placed on the market ([[CRA Article 13(5)]], [[official/faq_4-4-1]]). Whether a component arrived as a library, a package, a container image, an SDK, a copy pasted into your repository or a dependency of a dependency does not matter: if it ships in the product, you answer for it.

The SBOM has a narrower minimum. It has to cover _"at the very least the top-level dependencies"_ of the product ([[CRA Annex I, Part II]]), which is a floor for the document, not a limit on your responsibility: a vulnerability in a dependency three levels down is still a vulnerability in your product.

How much checking each component gets depends on its risk. The Commission's FAQ lists what due diligence can consist of, from checking a CE marking or a security update history to reviewing the component's SBOM, checking its support period and running your own tests ([[official/faq_4-4-2]]; see [[due-diligence/what-is-due-diligence]] and [[due-diligence/foss]]). A component that is itself a CRA product lets you rely on its manufacturer's declaration; one that is not, which is most open source, needs other means ([[official/faq_4-4-1]]).

Tooling that does not ship in the product, such as compilers and test frameworks, is not a component of it, and neither the CRA nor the guidance addresses it beyond that; what it could do to what you ship is a matter for your risk assessment ([[CRA Article 13(2)]]). A component you have copied in and patched is yours to handle like any other, and the fix you make to it is shared with the project it came from ([[CRA Article 13(6)]]). An upstream project's own SBOM helps as input: see [[manufacturers/upstream-sbom]].
