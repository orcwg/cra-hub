---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/128
---

# How does the support period of a framework or component relate to the products built on it?

Each manufacturer sets the support period of its own product, and the two periods inform each other without one being derived from the other. The manufacturer of a framework or runtime component sets its period from the time its product is expected to be in use, judged by reasonable user expectations, the nature and intended purpose of the product and any EU law on its lifetime ([[CRA Article 13(8)]], [[official/faq_4-5-1]]). For a component meant to be built into other products, that expected use includes the years those products will be sold and used, which is why five years _"is not to be considered as the default"_ and longer periods are expected where products are in use longer ([[CRA-GUIDANCE point 126]], [[CRA Recital 60]]; see [[manufacturers/support-period]]).

The manufacturer of the product built on the framework sets its own period the same way, and _may_ take the framework's support period into account, as one of the factors the CRA lists alongside the support periods of similar products and the availability of the operating environment ([[CRA Article 13(8)]], [[official/faq_4-3-7]]). It can rely on the framework's manufacturer handling vulnerabilities in the framework for as long as that period runs ([[official/faq_4-3-6]]).

What the law does not do is let the product's period shorten to the framework's. Where a product is still supported and a vulnerability appears in a component whose own support has ended, the product's manufacturer has to remediate it by other means, by replacing the component or patching it itself ([[official/faq_4-3-7]]; see [[manufacturers/unmaintained-component]]). So the framework's period is a reason to choose that framework, or to plan for the day it ends, not a ceiling on what the product owes its users.

For a framework released in successive versions, each substantially modified version placed on the market gets its own period, and support for earlier versions may stop once users can upgrade free of charge and without additional costs ([[CRA Article 13(10)]], [[CRA-GUIDANCE point 130]], [[CRA-GUIDANCE point 131]]).
