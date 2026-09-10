---
Status: ⚠️ Draft
Related issues: https://github.com/orcwg/cra-hub/issues/32
---

# Do I need to notify ENISA of every vulnerability in my product? I have heard about a 24 hour rule.

No. Only two things trigger a mandatory notification under [[Article 14]]:

* an _actively exploited vulnerability_ in your product, meaning there is evidence that a malicious actor is using it against real systems, see [[Article 14(1)]]. An internal finding, a researcher report, a proof of concept or a high severity score does not by itself trigger the duty (see [[Recital 66]] to [[Recital 68]]); and
* a _severe incident_ having an impact on the security of your product, see [[Article 14(3)]].

The "24 hour rule" is the first stage of a three stage cascade. Every clock runs from the moment you become aware.

| Stage | Deadline | What you submit |
| - | - | - |
| Early warning[^1] | 24 hours | Notification to your [relevant CSIRT][] and to [ENISA][] through the [Single Reporting Platform][srp] |
| Notification[^2] | 72 hours | General information about the product, the nature of the exploitation or incident, and any corrective or mitigating measures taken |
| Final report[^3] | 14 days after a corrective measure is available | Full report; one month for severe incidents |

You must also inform impacted users, and where appropriate all users, through available channels, see [[Article 14(8)]].

These obligations apply from 11 September 2026, ahead of the rest of the regulation ([[Article 71]]), and they cover products already on the market rather than only newly placed ones.

Everything below that threshold stays in your normal vulnerability handling process — coordinated disclosure, advisories, CVE assignment — which [[Annex I]] Part II requires from December 2027 anyway. Voluntary notification of other vulnerabilities and near misses remains possible under [[Article 15]].

For the equivalent obligations of _open-source software stewards_, which are a subset of these, see [notification obligations of stewards][stewards].

[^1]: [[Art. 14(1)]] and [[Art. 14(3)]]
[^2]: [[Art. 14(2)]]
[^3]: [[Art. 14(2)]]

[relevant CSIRT]: ../vulnerability-handling/csirt.md
[ENISA]: ../vulnerability-handling/enisa.md
[stewards]: ../stewards/notification-obligations.md
[srp]: https://www.enisa.europa.eu/topics/product-security-and-certification/single-reporting-platform
