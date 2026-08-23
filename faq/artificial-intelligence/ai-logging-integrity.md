---
Status: ⚠️ Draft
Related issues: TBD (open a tracking issue for the AI / AI-agents FAQ section)
Source: Annex I, Part I, point (2)(l)
---

# What does the CRA require me to log for an AI system, and do the logs need to be tamper-proof?

The CRA's logging requirement is in Annex I, Part I, point (2)(l): a product must "provide security related information by recording and monitoring relevant internal activity, including the access to or modification of data, services or functions, with an opt-out mechanism for the user."

What counts as relevant internal activity is not defined for an AI agent, but it is enumerable. The classes an agent produces include tool and function calls together with their arguments; the content returned by tools and by retrieval, which is a primary channel for prompt injection; reads and writes against memory or context; and requests that cross a trust boundary. That list is illustrative rather than exhaustive, and it describes what an agent does rather than prescribing what a manufacturer must record. Enumerability is the practical point: a logging requirement nobody can enumerate is one two vendors will implement very differently while both claim conformity. Where the category boundary sits would benefit from Commission guidance or a harmonised standard. Open prior art shows the decomposition is practicable rather than merely arguable — the MIT-licensed [agent-threat-rules SPEC](https://github.com/Agent-Threat-Rule/agent-threat-rules/blob/fd0f67f07ab969b025f0074f5e21532638e21568/SPEC.md) defines an `AgentEvent` covering LLM input and output, tool calls and context-window state, keeps its event-class enum open for extension, and carries a trust-boundary section (§13.1). It is third-party work, cited here as evidence of feasibility and pinned to a commit so the reference does not move; it is not an endorsement and the FAQ takes no position on it.

Notably, neither this point nor the rest of Annex I requires that those logs be cryptographically protected, tamper-evident, or time-anchored against later alteration — the requirement is about recording and monitoring, not about the integrity of the log itself. (Point (2)(f) does address integrity, but of the data, commands, programs and configuration the product handles, not specifically of the security log.) How to make recorded activity independently verifiable is therefore not spelled out in the text, and may be an area where guidance or standardisation is useful.

If your product is also a high-risk AI system, separate record-keeping duties apply under Article 12 of the AI Act, which address logging capability and content rather than log integrity.
