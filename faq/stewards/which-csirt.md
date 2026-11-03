---
Status: ✅ Approved
guidance-id: csirt-identification
Related issues: https://github.com/orcwg/cra-hub/issues/167
---

# Which CSIRT does an open source steward outside the EU report to?

An open source steward with no establishment in the EU reports to the CSIRT of the EU country where, as far as it can tell, its project has the most users, and it may keep reporting to that same CSIRT afterwards.

Stewards involved in a project's development report actively exploited vulnerabilities the way manufacturers do ([[CRA Article 24(3)]]), and that includes the rule for choosing the CSIRT: the notification goes to the _CSIRT designated as coordinator_ _"in accordance with paragraph 7"_ of [[CRA Article 14]] ([[CRA Article 14(1)]], [[CRA Article 14(7)]]). ENISA confirms that stewards, once their reporting obligations apply, are _"responsible for identifying the correct CSIRT designated as coordinator (CDaC) in accordance with Art. 14(7) of the CRA and selecting it when submitting a notification through the SRP"_ ([[srp/faq_18]]). What a CSIRT is, and the list of them: see [[vulnerability-handling/csirt]].

[[CRA Article 14(7)]] works in two steps:

- If you have a _main establishment_ in the EU, report to the CSIRT of the EU country where the decisions about the cybersecurity of your software are predominantly taken; if that cannot be determined, the country where you have the most employees in the EU. A steward headquartered outside the EU but with an EU office where those decisions are taken falls here.
- If you have no main establishment in the EU, the regulation lists four fallbacks in order, _"based on the information available"_ to you: the country of your authorised representative, of your importer, of your distributor, and finally _"the Member State in which the highest number of users"_ of your software are located ([[CRA Article 14(7)(d)]]).

For a steward, the first three fallbacks normally do not apply: a steward has no authorised representative (see [[stewards/authorised-representative]]), and software that is published without being sold has no importer or distributor in the CRA's sense, since both are defined by placing or making a product available on the EU market ([[CRA Article 3(16)]], [[CRA Article 3(17)]], [[CRA-GUIDANCE point 71]]). That leaves the country with the most users. You only need your best estimate from the information you have, and once you have reported to that CSIRT, you may send later notifications to the same one ([[CRA Article 14(7)]]). Choose with some care: ENISA says a notification sent to the wrong CSIRT _"may be invalidated and will need to be resubmitted to the correct CDaC"_ ([[srp/faq_18]]). The CSIRTs and ENISA run a helpdesk for reporting questions ([[CRA Article 17(6)]], [[srp/faq_19]]).

The Commission's guidance confirms that stewards report actively exploited vulnerabilities they become aware of ([[CRA-GUIDANCE point 216]]) but says nothing more about how a steward chooses its CSIRT, and a project that does not know where its users are has little to go on. The hub has asked the Commission for criteria that stewards can rely on, and for a fallback with ENISA when a steward cannot identify its CSIRT: see [[pending-guidance/csirt-identification]].

Reporting obligations for stewards apply from 11 December 2027 ([[official/faq_5-5]]), and only to stewards involved in a project's development or providing the infrastructure it is developed on: see [[stewards/notification-obligations]].
