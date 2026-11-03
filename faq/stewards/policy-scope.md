---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/312
---

# Does the steward's cybersecurity policy apply to how the project is developed, or to how others integrate it into their products?

The steward's cybersecurity policy applies to how the open source project itself is developed and how its vulnerabilities are handled, not to how other companies integrate the project into their products.

[[CRA Article 24(1)]] requires stewards to put in place _"a cybersecurity policy to foster the development of a secure product with digital elements as well as an effective handling of vulnerabilities by the developers of that product"_. The _product with digital elements_ here is the open source project the steward supports, and _"the developers of that product"_ are its maintainers and contributors. Everything the article says the policy must cover is about the project's own practices: documenting, addressing and remediating vulnerabilities, encouraging the project's developers to report vulnerabilities voluntarily under [[CRA Article 15]], and sharing information about discovered vulnerabilities _"within the open-source community"_ ([[CRA Article 24(1)]]). The policy also has to fit the steward's own nature and the legal and organisational arrangements it works under, such as how much of the project's development it is involved in ([[CRA Article 24(1)]], [[CRA-GUIDANCE point 79]]).

The Commission's guidance reads the policy the same way: it is what a steward follows when it passes a vulnerability reported from outside on to _"the maintainers of the product with digital elements"_, and it should _"foster the correct handling of vulnerabilities"_ within the project ([[CRA-GUIDANCE point 80]], [[CRA-GUIDANCE point 81]]).

Making the project easy to integrate securely, with safe defaults and good documentation for the companies that build on it, is not something the CRA requires of a steward. Maintainers of open source software that is not sold _"do not bear obligations in relation to other entities that may integrate such components into their products with digital elements"_ ([[CRA-GUIDANCE point 87]]). The companies that integrate the project are responsible for their own products and have to do their own due diligence on the components they use ([[CRA Article 13(5)]], [[CRA-GUIDANCE point 88]]). Help for integrators belongs instead to the voluntary security attestation programmes the Commission may set up to make that due diligence easier ([[CRA Article 25]], [[CRA Recital 21]]): see [[attestations/what-is-a-security-attestation]] (they do not exist yet) and [[due-diligence/support]] (how a project can support manufacturers' due diligence). Nothing stops a steward's policy from encouraging secure integration as well; it is just not required.

Separately from the policy, a steward may still have to notify actively exploited vulnerabilities and inform the project's users, depending on how involved it is in development: see [[stewards/notification-obligations]].
