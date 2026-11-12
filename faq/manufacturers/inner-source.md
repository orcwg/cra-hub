---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/365
---

# Are inner source maintainers manufacturers under the CRA?

No. The maintainers of an inner source project are never its manufacturers: the CRA's obligations fall on the company that supplies a product, as a legal person, not on the employees who write or maintain the code ([[CRA Article 3(13)]]; see [[cra-itself/projects-or-persons]]). Whether the company is the manufacturer of an inner source project depends on where the code goes.

Within one company, inner source is software made for the company's own use, and the Commission's FAQ says placing on the market _"is considered not to take place where a product is manufactured for one's own use"_ ([[official/faq_1-5]]). The project is not a product under the CRA and has no obligations of its own. The products the company sells, built from it, do: the essential requirements apply to each of them as a whole, inner source code included ([[CRA Article 13(1)]], [[CRA-GUIDANCE point 173]]).

Across the legal entities of a group, the code is supplied from one legal person to another. That is a supply in the course of a commercial activity, with or without payment, and it places the software on the market ([[CRA Article 3(22)]]; see [[manufacturers/intra-group]]). The entity supplying it is then its manufacturer, with a manufacturer's obligations for it ([[CRA Article 13]]), and the entities building it into their products owe due diligence on it as a component ([[CRA Article 13(5)]]).

The open source rules do not apply. Inner source is not free and open source software under the CRA, whose definition requires source code that is _"openly shared"_, meaning publicly available, under a free and open source licence ([[CRA Article 3(48)]], [[CRA-GUIDANCE point 46]]). Neither the exemption for open source that is not monetised nor the steward role is open to an inner source project. They become available if the company publishes the project as open source: see [[stewards/own-software]].
