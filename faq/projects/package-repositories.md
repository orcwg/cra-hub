---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/257
---

# Does our package repository or distribution become a distributor under the CRA when a package we carry is monetised?

No, a package repository or distribution does not become a _distributor_ under the CRA because the maintainer of one of its packages starts to monetise it. The CRA says that _"the sole act of hosting products with digital elements on open repositories, including through package managers or on collaboration platforms"_ is not making them available on the market. The organisation running such a service is a distributor only if it supplies the software in the course of its own commercial activity ([[CRA Recital 20]], [[CRA Article 3(17)]], [[CRA Article 3(22)]]). The maintainer's commercial activity does not pass to it. This holds alike for language registries such as PyPI or CPAN, Linux and BSD distributions, and container registries. Neither the Commission's guidance nor its FAQs mentions them specifically.

Often the package in the repository is not the monetised product anyway. Selling support for a project that stays free does not place the project on the market, and when a version is reserved for paying customers, the free version remains a separate product: see [[manufacturers/paid-support]].

Your organisation's own activity decides its role. A volunteer-run distribution that redistributes packages without monetising them has no commercial activity, so the CRA asks nothing of it as a distributor. A company that sells a distribution, or charges for access to its packages or their updates, is the manufacturer of the product it markets under its name ([[CRA Article 3(13)]], [[CRA Article 21]]). A company that resells another manufacturer's product unchanged is that product's distributor, and checks that it bears the CE marking before supplying it ([[CRA Article 20(2)(a)]]).

An organisation that hosts and sustains open source projects without selling them may instead be their _open-source software steward_: hosting source code or software is one of the forms of support the CRA lists ([[CRA Recital 19]], [[CRA-GUIDANCE point 75]]). See [[stewards/sustained-support]].
