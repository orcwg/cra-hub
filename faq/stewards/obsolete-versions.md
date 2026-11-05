---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/354
---

# Do a steward's reporting obligations cover vulnerabilities in obsolete versions of a project?

A steward's reporting obligations do not cover a version once it has reached its end of life. Stewards report actively exploited vulnerabilities only _"to the extent that they are involved in the development"_ of the software ([[CRA Article 24(3)]]). And they are stewards only of software _"intended for commercial activities"_ ([[CRA Article 3(14)]]). A version is no longer developed, nor meant for anyone to build products on, once the project stops maintaining it. It is no longer stewarded, so there is nothing to report on it. A version still maintained is covered, however old it is.

The guidance says that where an organisation _"ceases to provide systematic support on a sustained basis for a specific FOSS, it may no longer meet the definition of steward"_ ([[CRA-GUIDANCE point 83]]). The organisation should then _"communicate clearly the change in its status"_ ([[CRA-GUIDANCE point 83]]). Stopping support for one version works the same way as stopping support for a whole project: see [[stewards/inactive]].

The project itself decides which versions are still covered, by declaring a version's end of life where users will see it. The declaration also tells users of the obsolete version that running unsupported software carries a risk, as the CRA asks of manufacturers' software archives ([[official/faq_1-7]]). Selling security updates for an obsolete version is monetising it. That makes the seller the version's manufacturer ([[CRA-GUIDANCE point 57]]).

For projects that predate the CRA, see [[stewards/old-projects]]; for what a steward reports, [[stewards/notification-obligations]].
