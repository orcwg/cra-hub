---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/167
---

# Does an open source steward outside the EU need an authorised representative in the EU?

No, an open source steward based outside the EU does not need an authorised representative in the EU. Neither the Commission's FAQ nor its guidance on stewards ([[CRA-GUIDANCE Section 3.3]]) addresses the question, but the CRA only lets a _manufacturer_ appoint one, and this is the hub's reading of it: an _authorised representative_ is a person or company established in the EU that a manufacturer has mandated in writing to act on its behalf, and even a manufacturer only _"may"_ appoint one ([[CRA Article 3(15)]], [[CRA Article 18(1)]]). The tasks a mandate covers, keeping the technical documentation and the EU declaration of conformity and handing them to the market surveillance authorities, are manufacturers' tasks that a steward does not have ([[CRA Article 18(3)]]).

What a steward has to do is listed in [[CRA Article 24]]: put in place and document a cybersecurity policy, cooperate with market surveillance authorities when they ask, and, depending on how involved it is in a project's development, report actively exploited vulnerabilities and severe incidents ([[CRA Article 24(3)]], [[CRA-GUIDANCE point 79]]). None of this depends on where the steward is based: the definition of a steward requires a _legal person_ (a company or a foundation) but says nothing about where it is established ([[CRA Article 3(14)]]).

A foundation in the United States or a company in Switzerland that stewards a project therefore deals with the EU directly: it answers a reasoned request from a market surveillance authority itself, in a language the authority can easily understand ([[CRA Article 24(2)]]), and, where it has to report, it reports itself through ENISA's single reporting platform, which ENISA describes as _"an online tool for manufacturers and open-source software stewards"_ ([[srp/faq_1]]). The platform's _Assigned Representatives_ are something else: the people who register on it with their own EU Login account and file the steward's notifications ([[srp/faq_9]]), not a representative in the CRA's sense. Which national CSIRT a steward with no establishment in the EU reports to: see [[stewards/which-csirt]]. Which stewards have to report at all: see [[stewards/notification-obligations]].
