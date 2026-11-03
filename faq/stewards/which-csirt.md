---
Status: ✅ Approved
guidance-id: csirt-identification
Related issues: https://github.com/orcwg/cra-hub/issues/167
---

# Which CSIRT does an open source steward outside the EU report to?

An open source steward with no establishment in the EU reports to the CSIRT of the EU country where, as far as it can tell, its project has the most users, and it may keep reporting to that same CSIRT afterwards. ENISA's FAQ on the reporting platform answers the question for manufacturers and stewards alike: _"Manufacturers and, once applicable, open-source software stewards are responsible for identifying the correct CSIRT designated as coordinator (CDaC) in accordance with Art. 14(7) of the CRA and selecting it when submitting a notification through the SRP"_ ([[srp/faq_18]]). What a CSIRT is, and the list of them: see [[vulnerability-handling/csirt]].

ENISA sets out the rule of [[CRA Article 14(7)]] in two steps ([[srp/faq_18]]):

- _"In general, you should report to the CDaC in the Member State of your main establishment in the EU"_, which is _"the place where decisions related to the cybersecurity of your products with digital elements are predominantly taken"_; if that cannot be determined, the EU country where you have the most employees. A steward headquartered outside the EU but with an EU office where those decisions are taken falls here.
- If you have no main establishment in the EU, four fallbacks apply in order, _"based on the information available"_: the EU country of your authorised representative, of your importer, of your distributor, and _"if none of the above applies, the Member State with the highest number of users of your products with digital elements"_.

ENISA does not say how those fallbacks play out for a steward. The hub's reading is that the first three normally do not apply: a steward has no authorised representative (see [[stewards/authorised-representative]]), and software that is published without being sold has no importer or distributor in the CRA's sense, since both are defined by placing or making a product available on the EU market ([[CRA Article 3(16)]], [[CRA Article 3(17)]], [[CRA-GUIDANCE point 71]]). That leaves the country with the most users. You only need your best estimate from the information you have, and once you have reported to that CSIRT, you may send later notifications to the same one ([[CRA Article 14(7)]]). Choose with some care: ENISA says a notification sent to the wrong CSIRT _"may be invalidated and will need to be resubmitted to the correct CDaC"_ ([[srp/faq_18]]). The CSIRTs and ENISA run a helpdesk for reporting questions ([[srp/faq_19]], [[CRA Article 17(6)]]).

The Commission's guidance confirms that stewards report actively exploited vulnerabilities they become aware of ([[CRA-GUIDANCE point 216]]) but says nothing about how a steward chooses its CSIRT, and a project that does not know where its users are has little to go on. The hub has asked the Commission for criteria that stewards can rely on, and for a fallback with ENISA when a steward cannot identify its CSIRT: see [[pending-guidance/csirt-identification]].

Reporting obligations for stewards apply from 11 December 2027 ([[official/faq_5-5]], [[srp/faq_29]]), and only to stewards involved in a project's development or providing the infrastructure it is developed on: see [[stewards/notification-obligations]].
