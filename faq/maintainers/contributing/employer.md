---
canonical-id: maintainers/employer
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/298
---

# If you maintain an open source project in your own time and work for a company, does the CRA apply to you or your employer?

No, neither of you has obligations under the CRA for a project you maintain in your own time and don't monetise, even if your open source work helped you get the job. You publish the project for free, so it is not placed on the market and the CRA does not apply to you ([[CRA-GUIDANCE point 53]]; see [[maintainers/no-monetization]]). Your employer is not involved: open source software is under the responsibility of those who _"publish it and exercise primary control over its development, releases, and distribution decisions"_ ([[CRA-GUIDANCE point 49]]), and a project you run outside your employer's supervision is under yours, not theirs. That your reputation as a maintainer counted in hiring you is not monetising the project: how a project's work is financed does not count ([[CRA Recital 18]]; see [[maintainers/paid-dev]]).

That changes if your employer takes the project on. If the company sells it, as a paid version or a product built on it, the company is the manufacturer of what it sells ([[CRA-GUIDANCE point 57]]; see [[manufacturers/what-is-a-manufacturer]]). If it takes over the project itself, publishing it and controlling its releases, and keeps it free, it may become the project's _open-source software steward_, since the steward role falls on companies that systematically support software meant for commercial use ([[CRA Article 3(14)]]; see [[stewards/business-context]]).

If your employer only depends on your project, building it into products it sells, your position does not change either. The company has to exercise due diligence on your project as a component and report to you the vulnerabilities it finds in it; you owe it nothing in return ([[CRA-GUIDANCE point 87]], [[CRA-GUIDANCE point 88]]; see [[maintainers/used-in-products]]). Merging your employer's patches into your own project on company time is where the line gets thin: see [[cra-itself/under-responsibility]] for what moves a project under a company's control.
