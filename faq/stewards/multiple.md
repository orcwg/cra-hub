---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/22
---

# Can a project have multiple stewards?

Yes, nothing in the CRA stops a project from having more than one steward, but it is rare and usually not worth it.

A steward is a company or foundation (a _legal person_) that systematically provides sustained support for a specific open source project and ensures its viability ([[CRA Article 3(14)]]). The CRA sets no limit on how many organisations can play that role for the same project, and the Commission's guidance doesn't address the question: it looks at each organisation and each project separately ([[CRA-GUIDANCE point 72]], [[CRA-GUIDANCE point 74]]). Every organisation that meets the definition for a project is a steward of it, with a steward's obligations.

Few organisations meet it, though. The guidance ties the steward role to the organisation that publishes the project and exercises _"primary control over its development, releases, and distribution decisions"_ ([[CRA-GUIDANCE point 71]], [[CRA-GUIDANCE point 49]]). A company that contributes code, developer time or money to a project someone else publishes is a contributor, not a steward, however much it contributes ([[CRA Recital 18]], [[CRA-GUIDANCE point 85]], [[CRA-GUIDANCE point 86]]). In every example the guidance gives, a project has one steward, the foundation or company that publishes it, and the companies contributing to it have no obligations for it ([[CRA-GUIDANCE Example 28]], [[CRA-GUIDANCE Example 31]], [[CRA-GUIDANCE Example 33]]). So a foundation hosting a project that a company started and still contributes to has one steward, the foundation. Two stewards only arise where two organisations both publish and sustain the same project.

Even then, each steward has to put in place its own cybersecurity policy for the project, answer market surveillance authorities about it and report actively exploited vulnerabilities and severe incidents ([[CRA Article 24]]; see [[stewards/obligations]]). A project whose developers answer to two security policies and two reporting lines is harder to run than one with a single steward clearly responsible for it. If several organisations support your project, the simplest arrangement is for one of them to publish and govern it as its steward and for the others to contribute: see [[stewards/relationship]] and [[stewards/foundation]]. An organisation that stops supporting a project stops being its steward, and should say so ([[CRA-GUIDANCE point 83]]).
