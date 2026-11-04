---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/63
---

# Which existing practices should an open source project adopt now to prepare for the CRA?

The practices worth adopting now are the ones the CRA writes into law for manufacturers in its vulnerability handling requirements ([[CRA Annex I, Part II]]), most of which open source projects already know as good practice. A project that is not in scope has no obligation to adopt any of them; they help because the companies that build your project into their products have to check these things as part of their due diligence ([[official/faq_4-4-2]]), and because a steward's cybersecurity policy is built from them ([[CRA Article 24(1)]]).

From [[CRA Annex I, Part II]], the practices are:

- **A software bill of materials (SBOM)** in a commonly used, machine-readable format, covering at least your top-level dependencies.
- **A coordinated vulnerability disclosure policy** and a contact address for reporting vulnerabilities, typically a `SECURITY.md`. The Commission's guidance says manufacturers who find a vulnerability in your project should report it through the channels you publish ([[CRA-GUIDANCE point 223]]) and share fixes the way your guidelines ask ([[CRA-GUIDANCE point 227]]).
- **Security advisories** once a fix is out, describing the vulnerability, the affected versions, its severity and how to remediate it.
- **Security updates without delay**, separate from feature updates where feasible, and **securely distributed**, for example signed releases.
- **Regular security tests and reviews** of the code.

Doing these is what manufacturers check when they integrate a component: its security update history, known vulnerabilities, its SBOM and its support period ([[official/faq_4-4-2]]). What documentation helps them: see [[due-diligence/support]]. Whether the CRA applies to your project at all: see [[maintainers/should-i-worry]].
