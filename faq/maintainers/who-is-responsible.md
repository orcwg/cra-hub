---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/18
---

# Who is responsible for an open source project under the CRA when no single person or company controls it?

Under the CRA, an open source project is the responsibility of the people who publish it and have primary control over its development, releases and distribution, whatever the project's governance: not its copyright holders, and not everyone with commit access.

The Commission's guidance says this directly, with projects like yours in mind, _"which often involves multiple contributors, decentralised collaboration models and a separation between contribution and decision-making"_: open source software is _"under the responsibility"_ of the _"natural or legal persons who publish it and exercise primary control over its development, releases, and distribution decisions (often referred to as 'maintainers')"_ ([[CRA-GUIDANCE point 49]]). People who contribute code but _"do not control releases, roadmaps, or governance decisions"_ are contributors, and the project is not their responsibility even though their code is in it ([[CRA Recital 18]], [[CRA-GUIDANCE point 49]], [[CRA-GUIDANCE Example 13]], see [[maintainers/contributors]]). Nor do permissions settle it: _"the mere existence of technical permissions, such as commit access, is not sufficient to establish that the FOSS is under that person's responsibility"_ ([[CRA-GUIDANCE point 49]]). Neither the CRA nor the guidance mentions copyright at all: who wrote or owns the code is not the test, see [[stewards/whose-codebase]].

Being responsible for the project is not the same as having obligations. Those depend on what the responsible people do with it:

- If the project is not monetised, nobody is its manufacturer, and if the people who run it are individuals, nobody has obligations under the CRA ([[CRA-GUIDANCE point 53]], [[CRA-GUIDANCE point 87]], [[CRA-GUIDANCE Example 27]]). A group of maintainers with no legal entity behind it cannot be a steward either, because a steward has to be a company, foundation or similar legal person ([[CRA Article 3(14)]], see [[maintainers/multiple-maintainers-steward]]).
- A foundation or company that supports the project on a sustained basis, by hosting it, governing it, steering its development or employing its developers, can be its open-source software steward if the project is intended for commercial use ([[CRA Article 3(14)]], [[CRA Recital 19]], [[CRA-GUIDANCE point 75]], [[CRA-GUIDANCE point 78]], [[CRA-GUIDANCE point 79]]). See [[stewards/whose-codebase]] and [[stewards/relationship]].
- Whoever supplies a monetised version of the project under their own name, such as a company selling a supported build, is the manufacturer of that version, and of that version only ([[CRA Article 3(13)]], [[CRA-GUIDANCE point 51]], [[CRA-GUIDANCE point 52]], [[CRA-GUIDANCE Example 30]]). It does not make the community that runs the project a manufacturer. See [[maintainers/become-manufacturer]].

Neither the CRA nor the guidance addresses a group of individuals with no legal entity behind it that monetises a project together.
