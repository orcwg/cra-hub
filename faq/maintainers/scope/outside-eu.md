---
canonical-id: maintainers/outside-eu
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/79
---

# I'm a solo maintainer not based in the EU. What impact does the CRA have on me?

The same as on a solo maintainer in the EU: none, unless you monetise your project and supply it to the EU market. Where you live does not enter into it. The CRA applies to products with digital elements _"made available on the market"_, meaning supplied for distribution or use _"on the Union market in the course of a commercial activity"_ ([[CRA Article 2(1)]], [[CRA Article 3(22)]]), wherever the person supplying them is based.

If you don't monetise your project, you are outside the CRA: the Commission's guidance says that open source software an individual provides for free _"is not within the scope of the CRA"_ ([[CRA-GUIDANCE point 53]]). Donations and paid support that cover your costs do not count as monetising: see [[maintainers/donations]] and [[maintainers/living-expenses]].

If you do monetise it and people in the EU get it, you are its manufacturer with the same obligations as a manufacturer in the EU ([[CRA Article 13]]; see [[maintainers/become-manufacturer]]). Two things are specific to being outside the EU: you may, but need not, appoint an _authorised representative_ established in the EU to deal with authorities on your behalf ([[CRA Article 18(1)]]), and when you have to report an actively exploited vulnerability you report to the CSIRT of the EU country where your software has the most users, unless you have an EU establishment or representative ([[CRA Article 14(7)]]; see [[vulnerability-handling/csirt]]).

The obligations of an _open-source software steward_ do not reach you either, in or outside the EU: they fall on organisations, not individuals ([[CRA Article 3(14)]]; see [[maintainers/solo-maintainer-steward]]). For whether any of this is something to worry about, see [[maintainers/should-i-worry]].
