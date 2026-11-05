---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/81
---

# I'm a solo maintainer. Should I incorporate to avoid liability from the CRA?

No. As a solo maintainer of an open source project you don't monetise, you have no liability under the CRA to avoid: the CRA does not apply to you (see [[maintainers/no-monetization]]). Incorporating protects you from nothing under it, and can give you obligations you don't have today.

A company is a _legal person_, and the steward role exists only for legal persons: an _open-source software steward_ is a company or foundation, other than a manufacturer, whose purpose is to systematically support specific open source software intended for commercial use ([[CRA Article 3(14)]]). An individual publishing a project for free is _"not within the scope of the CRA"_, while a legal person doing the same is _"subject to the obligations on stewards"_ ([[CRA-GUIDANCE point 53]]). So a company you set up to hold a project that companies build on could become its steward, with the obligations of [[CRA Article 24]]: a cybersecurity policy, cooperation with authorities and vulnerability reporting. Stewards cannot be fined ([[CRA Article 64(10)(b)]]), but the obligations are real. See [[maintainers/solo-maintainer-steward]] and [[stewards/obligations]].

If you monetise your project, you are its manufacturer whether you are an individual or a company ([[CRA Article 3(13)]]; see [[manufacturers/individuals]]). Incorporating then makes the company the manufacturer, with the same obligations and the same fines, which already scale with size and, for an individual, with economic situation ([[CRA Article 64(5)(c)]], [[CRA Recital 121]]; see [[maintainers/penalties]]). Whether a company shields your personal assets from those fines is a question of company law in your country, not of the CRA.

Whether to incorporate is therefore a general business decision, to take on its own merits. For handing a project to an existing organisation instead, see [[maintainers/hand-to-steward]].
