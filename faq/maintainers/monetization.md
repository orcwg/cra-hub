---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/133, https://github.com/orcwg/cra-hub/issues/16
guidance-id: open-source-guidance
---

# Am I subject to the CRA if I earn a living from the open source project I maintain?

Not as long as what you earn from the project only covers your actual costs, which include a reasonable salary or [living expenses][] ([[CRA Recital 15]], [[CRA-GUIDANCE point 58]], [[CRA-GUIDANCE point 61]]). See [[cra-itself/actual-costs]] for what counts.

If you earn more than that by charging for the open source software itself, you are monetising it, and the CRA treats you as its manufacturer, with the obligations of [[CRA Article 13]]:

- **Charging for the software**: a price for the software or for its binaries ([[CRA-GUIDANCE point 51]]), or updates, maintenance or technical assistance reserved for paying users ([[CRA-GUIDANCE point 57]]). For an individual, a supported version whose price only recovers actual costs is the exception ([[CRA-GUIDANCE point 58]]).
- **Donations taken with the intention of making a profit** ([[CRA Recital 15]]). Donations fluctuate, so a degree of flexibility applies, and a project supported only through donations is unlikely to be considered placed on the market; donations that are really the price of access are a sale ([[CRA-GUIDANCE point 61]], [[CRA-GUIDANCE point 62]]). See [[maintainers/donations]].

Money that is not for the software itself does not count, whatever the amount:

- **Sponsorship, grants or paid development** of features that you then release to everyone: how the development was financed does not count ([[CRA Recital 18]], [[CRA-GUIDANCE point 63]], [[CRA-GUIDANCE point 65]]).
- **Paid services around freely available software**, such as consulting, training, integration or optional support: these are services, not a sale of the software, as long as anyone can download, install and update it without paying ([[CRA-GUIDANCE point 56]], [[CRA-GUIDANCE Example 18]]). See [[maintainers/consultants]] and [[maintainers/technical-support]].

A paid product built on your project, such as an "enterprise" edition or an open-core product, is a different product. It is covered by the CRA like any other software you sell, whether or not its source is open, and you are its manufacturer. It does not change the status of the open source version: that stays outside the CRA if you are an individual, and makes you its open-source software steward if you are a company or foundation ([[CRA-GUIDANCE point 52]], [[CRA-GUIDANCE point 53]], see [[maintainers/solo-maintainer-steward]]). Note that software whose source code is only shared with paying customers is not open source under the CRA, whatever its licence ([[CRA Article 3(48)]], [[CRA-GUIDANCE point 46]]).

See [[cra-itself/monetisation]] for the other forms monetisation can take, such as monetising other services through the software or requiring users' personal data.

[living expenses]: ./living-expenses.md
