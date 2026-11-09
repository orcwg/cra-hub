---
canonical-id: maintainers/transparency
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/70
---

# If you are not subject to the CRA and want to make this clear to downstream users, what should you say?

Say that the project is not placed on the market, so neither the CRA nor the Product Liability Directive puts obligations on it towards the companies that use it, and that those companies' obligations run the other way. The Commission's guidance settles the first part: _"maintainers of FOSS components that are not placed on the market do not bear obligations in relation to other entities that may integrate such components into their products with digital elements"_ ([[CRA-GUIDANCE point 87]]). Manufacturers who integrate your project _"are required to comply with the CRA for their own products"_, owe due diligence on your project, and have to report vulnerabilities they find in it to you and share their fixes ([[CRA-GUIDANCE point 88]], [[CRA Article 13(5)]], [[CRA Article 13(6)]]). You are under no obligation to act on their reports or merge their fixes.

A reply you can adapt, for an individual or a project alike:

```markdown
- This project is open source software that is not monetised and so not placed on the market. On the basis of [Recital 18][] of the Cyber Resilience Act and the [Commission's guidance][] on it, it is outside the scope of the regulation, and its maintainers are neither manufacturers nor open-source software stewards under it.
- On the basis of [Recital 15 of the Product Liability Directive][PLD Recital 15], its maintainers cannot be held liable for your use of the code.
- While this project has no obligations towards you, you may have some towards it: on the basis of [Article 13(6)][] of the Cyber Resilience Act, if you believe you have found a vulnerability in this code, you are responsible for reporting it through the project's vulnerability disclosure process at <project link>, for fixing it in your product, and for sharing your fix with the project.

[Recital 18]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32024R2847#rct_18
[Commission's guidance]: https://cra.orcwg.org/official-guidance/#pnt_87
[PLD Recital 15]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32024L2853#rct_15
[Article 13(6)]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:32024R2847#art_13
```

Whether you are in fact outside the CRA: see [[maintainers/should-i-worry]] and [[maintainers/monetization]]. What integrators can expect from you: [[manufacturers/support-creates-obligations]].
