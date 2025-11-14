---
Status: ⚠️ Draft
Related issue: https://github.com/orcwg/cra-hub/issues/159, https://github.com/orcwg/cra-hub/issues/185
---

# What are the notification obligations of _open-source software stewards_?

Per [[Article 24(3)]], _open-source software stewards_ are subject to a subset of the notification obligations of manufacturers defined in [[Article 14]].

* If a steward is involved in the development of an open source project that it stewards, it must notify both its [relevant CSIRT][] and [ENISA][] of _any actively exploited vulnerability_ in that project, see [[Article 14(1)]].
* If a steward provides IT infrastructure used for the development of an open source project that it stewards, it must notify its [relevant CSIRT][] and [ENISA][] of _any severe incident_ having an impact on the security of that project, see [[Article 14(3)]].
* In both of those cases, it must inform impacted users (and where appropriate all users) of that open source project through available channels (e.g. changelog, blog post, mailing list, direct contact when available, etc.), see [[Article 14(8)]].

The table below provides an actionable summary of those notification and information obligations that accounts for stewards not necessarily being aware of who their users are nor being able to reach out to them individually.

| Steward support level | Notify vulnerabilities[^1] | Notify incidents[^2] | General announcement (e.g. changelog, blog post, mailing list, etc.)[^3] | Message known users directly[^3] |
| - |:-:|:-:|:-:|:-: |
| Provides non-technical support | N/A | N/A | N/A | N/A |
| + provides IT infrastructure | N/A | ✅ | ✅ | N/A |
| + provides engineering resources (incl. security) | ✅ | ✅ | ✅ | N/A |
| + has 1:1 relationship with some users (e.g. through enterprise edition, membership, etc.) | ✅ | ✅ | ✅ | ✅|

[^1]: [[Art. 14(1)]]
[^2]: [[Art. 14(3)]]
[^3]: [[Art. 14(8)]]

[relevant CSIRT]: ../vulnerability-handling/csirt.md
[ENISA]: ../vulnerability-handling/enisa.md
