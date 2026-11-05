---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/20, https://github.com/orcwg/cra-hub/issues/92
---

# What are the obligations of a manufacturer under the CRA?

A manufacturer has to place on the market a product that meets the CRA's essential cybersecurity requirements, keep handling the product's vulnerabilities for its support period, report actively exploited vulnerabilities and severe incidents, and document and declare all of it ([[CRA Article 13]], [[CRA Article 14]]). The obligations are the same for an open source product a company sells as for any other product.

Before placing the product on the market, the manufacturer assesses its cybersecurity risks and designs and builds it to the requirements of [[CRA Annex I, Part I]] in the light of that assessment ([[CRA Article 13(2)]], [[CRA Article 13(3)]]); exercises due diligence on the components it integrates, including open source ones ([[CRA Article 13(5)]]); draws up the technical documentation ([[CRA Article 31]]); carries out or commissions the conformity assessment ([[CRA Article 32]]); and then draws up the EU declaration of conformity, affixes the CE marking and supplies the product with the information and instructions of [[CRA Annex II]] ([[CRA Article 13(12)]]).

For the support period, at least five years ([[CRA Article 13(8)]]), it handles vulnerabilities as [[CRA Annex I, Part II]] requires: an SBOM, fixes without delay and security updates free of charge, a coordinated vulnerability disclosure policy and a contact address, secure distribution of updates, and public information on fixed vulnerabilities. A vulnerability it finds in a component is reported to whoever maintains the component, with any fix shared ([[CRA Article 13(6)]]). Security updates stay available for ten years, the documentation for ten years or the support period ([[CRA Article 13(9)]], [[CRA Article 13(13)]]).

An actively exploited vulnerability or a severe incident is reported through ENISA's single reporting platform, within 24 hours for the early warning ([[CRA Article 14]]; see [[vulnerability-handling/what-to-report]] and [[vulnerability-handling/deadlines]]).

The technical measures are the manufacturer's own choice, guided by its risk assessment; harmonised standards, once published, give a presumption of conformity ([[official/faq_4-2-1]]; see [[standards/harmonised-standards]]). For the conformity assessment, see [[manufacturers/self-assessment]]; for the support period, [[manufacturers/support-period]]; for components, [[due-diligence/foss]]; for what happens when a manufacturer falls short, [[manufacturers/mistakes]].
