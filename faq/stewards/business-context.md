---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/256
---

# What does 'intended for commercial activities' (or 'in a business context') mean in the steward definition?

Open source software is _"intended for commercial activities"_ when it is meant to end up in something that is sold. Neither the Commission's FAQ nor its guidance defines the phrase beyond the CRA's own words: the guidance says the steward concept applies to open source software that is _"ultimately intended for commercial activities, such as for integration into commercial services or into monetised products with digital elements"_, whether the organisation that publishes the software sells those products and services or other companies do ([[CRA-GUIDANCE point 71]], [[CRA Recital 19]]). What the guidance adds is cases, and the rest of this answer is drawn from them. "In a business context" is the same idea seen from the publisher's side: stewards include _"entities that develop and publish free and open-source software in a business context"_ ([[CRA Recital 19]]).

This condition only matters for companies and foundations. An individual cannot be a steward whatever their software is used for, and the Commission's guidance says that where the publisher is an individual, open source software that is not monetised _"is not within the scope of the CRA"_ at all ([[CRA Article 3(14)]], [[CRA-GUIDANCE point 53]]): see [[maintainers/solo-maintainer-steward]].

For a company or foundation, the Commission's guidance gives these cases of software intended for commercial activities:

- You built it for your own products or services, which you sell, and publish it as open source alongside them ([[CRA-GUIDANCE point 76]], [[CRA-GUIDANCE Example 25]], [[CRA-GUIDANCE Example 29]]).
- You publish it for other manufacturers to build into their products: a library, an SDK, a reference implementation ([[CRA-GUIDANCE point 67]], [[CRA-GUIDANCE Example 26]], [[CRA-GUIDANCE Example 33]]).
- Manufacturers who integrate it contribute to its development regularly, or fund it regularly to keep it going ([[CRA Recital 19]], [[CRA-GUIDANCE point 78]]).

What does not, by itself, make software intended for commercial activities:

- **Using it yourself at work.** Neither the Commission's FAQ nor its guidance addresses a tool you wrote for your own work and published on the side. The closest the FAQ comes is that tools a manufacturer develops for its own use are not in scope of the CRA unless it sells them separately ([[official/faq_1-5]]), and publishing them as open source without monetising them is not selling them ([[CRA Recital 18]], [[CRA-GUIDANCE point 42]]). The hub's reading is that such a tool is not intended for commercial activities either: using it in your own job is not building it into a service or product that customers get.
- **Publishing it under an open source licence.** Every open source licence allows commercial use. The guidance treats some of the software a foundation hosts as _"not intended for commercial activities"_, so the licence alone cannot be what decides ([[CRA-GUIDANCE point 78]]).
- **Someone else integrating it.** The Commission's guidance says the mere fact that manufacturers integrate your software into their products _"has no impact on the status of that FOSS component under the CRA"_ ([[CRA-GUIDANCE point 87]]). What the CRA counts is regular contributions or regular funding from the manufacturers who integrate it ([[CRA Recital 19]]).

Meeting this condition does not make your organisation a manufacturer: the Commission's guidance says you are a manufacturer only for software you actually sell or otherwise monetise ([[CRA-GUIDANCE point 74]]). It makes you a steward, with the lighter obligations of [[CRA Article 24]], provided your organisation also supports the project on a sustained basis: see [[stewards/sustained-support]] and [[stewards/obligations]].
