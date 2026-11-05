---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/77, https://github.com/orcwg/cra-hub/issues/74
---

# Does my project being used in commercial or critical products create obligations for me?

No. Your project being built into commercial products, including critical ones, creates no obligations for you under the CRA, whether you know about those uses or not. The Commission's guidance says that _"maintainers of FOSS components that are not placed on the market do not bear obligations in relation to other entities that may integrate such components into their products with digital elements"_: whether the CRA applies to your project depends only on whether you place it on the market ([[CRA-GUIDANCE point 87]]). The CRA does not look at who uses your project, how many, or how critical their products are: see [[maintainers/popularity]].

The obligations run the other way. A company that builds your project into a product it sells has to comply with the CRA for that product, exercise due diligence on your project as a component and, when it finds a vulnerability in your project, report it to you and share its fix ([[CRA Article 13(5)]], [[CRA Article 13(6)]], [[CRA-GUIDANCE point 88]], [[official/faq_4-4-4]]). An email from a car or medical device manufacturer is that company doing its due diligence. You are under no obligation to answer it, act on its reports or merge its fixes. What helps them, should you want to: [[projects/practices-to-adopt]] and [[due-diligence/support]]. How to tell them where you stand: [[maintainers/transparency]].

Two things do change your status, neither of them the use others make of your project. Monetising it makes you its manufacturer, and the category of what you sell then depends on its own core functionality, not on the products it ends up in: see [[maintainers/become-manufacturer]] and [[important-and-critical-products/what-qualifies]]. For a company or foundation that supports the project, learning that companies build on it bears on whether the project is intended for commercial use, one part of the steward definition: see [[stewards/business-context]]. An individual maintainer cannot be a steward: [[maintainers/solo-maintainer-steward]].
