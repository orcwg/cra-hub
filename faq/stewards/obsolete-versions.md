---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/354
---

# Do a steward's reporting obligations cover vulnerabilities in obsolete versions of a project?

No, not once a version has reached its end of life. A steward reports actively exploited vulnerabilities _"to the extent that they are involved in the development"_ of the software ([[CRA Article 24(3)]]), and is a steward of software _"intended for commercial activities"_ ([[CRA Article 3(14)]]). A version the project has stopped maintaining is no longer developed, nor meant for anyone to build products on. It is no longer stewarded, so there is nothing to report on it. A version still maintained is covered, however old it is.

Neither the CRA nor the Commission's guidance says this for stewards. The guidance says that for manufacturers the reporting obligation _"continues to apply after a product with digital elements is no longer supported"_ ([[CRA-GUIDANCE point 210]]), but a manufacturer's obligation attaches to a product it placed on the market, which does not change when support ends. A steward's attaches to its sustained support of the software, which does. The guidance says that where an organisation _"ceases to provide systematic support on a sustained basis for a specific FOSS, it may no longer meet the definition of steward"_, and encourages it to _"communicate clearly the change in its status"_ ([[CRA-GUIDANCE point 83]]). What it says of a whole project holds for a version: see [[stewards/inactive]].

What makes this hold is saying which versions are maintained. Declare end of life where users will see it, in the release policy or in a machine-readable statement in the [Common Lifecycle Enumeration (ECMA-428)][cle] or [OpenEoX][] format. Tell users of an obsolete version of the risk of running it, as the CRA asks of manufacturers' archives ([[official/faq_1-7]]). And an organisation that sells security updates for an obsolete version is monetising that version, which makes it a manufacturer of it ([[CRA-GUIDANCE point 57]]).

For projects that predate the CRA, see [[stewards/old-projects]]; for what a steward reports, [[stewards/notification-obligations]].

[cle]: https://ecma-international.org/publications-and-standards/standards/ecma-428/
[OpenEoX]: https://www.oasis-open.org/committees/openeox/
