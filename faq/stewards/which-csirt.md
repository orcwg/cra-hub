---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/167
---

# How do stewards outside the EU select which CSIRT to report to?

Stewards outside the EU select their CSIRT by the same rule as manufacturers, which for most of them means the CSIRT of the EU country where their software has the most users. ENISA says that _"manufacturers and, once applicable, open-source software stewards are responsible for identifying the correct CSIRT designated as coordinator (CDaC) in accordance with Art. 14(7) of the CRA"_ ([[srp/faq_18]]).

That rule points to the EU country of your _main establishment_, where decisions about your software's security are mostly taken, and otherwise to the country of your authorised representative, importer or distributor, or _"if none of the above applies, the Member State with the highest number of users"_ ([[CRA Article 14(7)]], [[srp/faq_18]]). A steward normally has none of the first three, so the last step applies; once you have reported to that CSIRT, you may keep reporting to it ([[CRA Article 14(7)]]).

Neither ENISA nor the Commission's guidance says what a steward that cannot tell where its users are should do: see [[pending-guidance/csirt-identification]]. What a CSIRT is: see [[vulnerability-handling/csirt]]. What stewards have to report: see [[stewards/notification-obligations]].
