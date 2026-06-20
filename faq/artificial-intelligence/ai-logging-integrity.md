---
Status: ⚠️ Draft
Related issues: TBD (open a tracking issue for the AI / AI-agents FAQ section)
Source: Annex I, Part I, point (2)(l)
---

# What does the CRA require me to log for an AI system, and do the logs need to be tamper-proof?

The CRA's logging requirement is in Annex I, Part I, point (2)(l): a product must "provide security related information by recording and monitoring relevant internal activity, including the access to or modification of data, services or functions, with an opt-out mechanism for the user." For an AI agent, the relevant internal activity plausibly includes the actions it takes and the tools it calls.

Notably, neither this point nor the rest of Annex I requires that those logs be cryptographically protected, tamper-evident, or time-anchored against later alteration — the requirement is about recording and monitoring, not about the integrity of the log itself. (Point (2)(f) does address integrity, but of the data, commands, programs and configuration the product handles, not specifically of the security log.) How to make recorded activity independently verifiable is therefore not spelled out in the text, and may be an area where guidance or standardisation is useful.

If your product is also a high-risk AI system, separate record-keeping duties apply under Article 12 of the AI Act, which address logging capability and content rather than log integrity.
