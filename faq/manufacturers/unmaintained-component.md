---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/111
---

# What do I do when an open source component in my product is no longer maintained?

The product stays yours to keep secure, component included. A manufacturer's vulnerability handling obligations apply to its product _"in their entirety, including to all integrated components"_, for the whole support period ([[official/faq_4-3-6]], [[CRA Article 13(8)]]). The people who developed a component that was never placed on the market have no obligations under the CRA, and when they are not there to help, the Commission's FAQ expects you to address a vulnerability _"via other means, for example by disabling compromised functions; switching out the affected component; developing by itself a patch"_ ([[official/faq_4-3-6]], [[official/faq_4-3-7]]). Which of these, and how fast, follows from the risk the vulnerability poses to your product ([[official/faq_4-3-1]]).

With nobody to report to, the Commission's guidance says you need not report the vulnerability upstream, but should still inform users of your product in another way ([[CRA-GUIDANCE point 225]]). If you patch the component and the project comes back to life, the patch is shared with it ([[CRA Article 13(6)]]).

A project that still exists but has stopped maintaining the version you use puts you in the same position for that version: you check whether the project's fix for newer versions applies to yours, backport it or move to a maintained version, and share what you backport ([[CRA Article 13(6)]]).

The time to think about this is when choosing components. A component's security update history and support period are part of due diligence ([[official/faq_4-4-2]]), and the support periods of components providing core functions are a factor in setting your product's own ([[official/faq_4-5-1]]; see [[manufacturers/component-support-period]]). Replacing the component, maintaining it yourself or funding its maintainers are all ways to meet the obligation; leaving a vulnerability unaddressed is not.
