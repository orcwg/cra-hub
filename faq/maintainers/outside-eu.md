---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/79
---

# I'm a solo maintainer not based in the EU. What impact does the CRA have on me?

The same as on a solo maintainer in the EU: none, unless you monetise your project and supply it to the EU market. Where you live does not enter into it. The CRA applies to products with digital elements _"made available on the market"_, meaning supplied for distribution or use _"on the Union market in the course of a commercial activity"_ ([[CRA Article 2(1)]], [[CRA Article 3(22)]]), wherever the person supplying them is based.

If you don't monetise your project, you are outside the CRA. The Commission's guidance says that where the person publishing open source software is an individual, the version provided for free _"is not within the scope of the CRA"_ ([[CRA-GUIDANCE point 53]]), and its example of an individual developer with a donation link ends with _"Developer A has no obligations under the CRA"_ ([[CRA-GUIDANCE Example 27]]). Donations and paid support that cover your costs, including your reasonable living expenses and a fair remuneration, do not count as monetising ([[CRA-GUIDANCE point 58]], [[CRA-GUIDANCE point 61]]): see [[maintainers/donations]] and [[maintainers/living-expenses]].

If you do monetise it and people in the EU get it, you are its manufacturer with the same obligations as a manufacturer in the EU ([[CRA Article 13]]; see [[maintainers/become-manufacturer]]). Two things are specific to being outside the EU: you may, but need not, appoint an _authorised representative_ established in the EU to deal with authorities on your behalf ([[CRA Article 18(1)]]), and when you have to report an actively exploited vulnerability you report to the CSIRT of the EU country where your software has the most users, unless you have an EU establishment or representative ([[CRA Article 14(7)]]; see [[vulnerability-handling/csirt]]).

The steward regime is not available to you as an individual, in or outside the EU: see [[maintainers/solo-maintainer-steward]]. Whether to worry at all: [[maintainers/should-i-worry]].
