---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/82
---

# Should I give my project to a steward to avoid obligations under the CRA?

No, not for that reason. The CRA does not apply to the maintainer of an open source project that is not monetised (see [[maintainers/no-monetization]]), so you have no obligations for a steward to take over. A steward has obligations of its own. It does not relieve anyone else of theirs.

An _open-source software steward_ is a company or foundation that systematically supports specific open source software meant for commercial use and keeps it viable ([[CRA Article 3(14)]]). It has those obligations because of the support it provides, from the moment it provides it ([[CRA-GUIDANCE point 70]]; see [[stewards/opt-in]]), and they cover its own conduct: a cybersecurity policy, cooperation with authorities, vulnerability reporting ([[CRA Article 24]]). Nothing in the CRA requires you to hand over your project for that. A foundation that hosts your repositories, runs your releases or handles your security reports can be its steward while you keep control of it ([[CRA-GUIDANCE point 79]]; see [[stewards/relationship]]). The project does not become the steward's, and you can change stewards.

If you monetise your project, you are its manufacturer, and no steward can take that over: a steward is by definition _"other than a manufacturer"_ ([[CRA Article 3(14)]], [[CRA-GUIDANCE point 71]]). What would change your obligations is to stop monetising, or for a company to sell it in your place and become its manufacturer.

What working with a steward does bring is support: infrastructure, security handling, funding, and the documentation that helps the companies building on your project do their due diligence ([[CRA-GUIDANCE point 79]]; see [[due-diligence/support]]). Those are reasons to seek one, and the choice is yours, by what the project needs. For setting up your own company instead, see [[maintainers/incorporate]].
