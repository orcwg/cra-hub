---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/94
---

# Can I use an SBOM published by an upstream project?

Yes, as input and as evidence, not as a substitute for the SBOM of your own product. A manufacturer has to draw up the SBOM of its product itself, covering at the very least the product's top-level dependencies ([[CRA Annex I, Part II]]). Reviewing the SBOM of a component, where one exists, is one of the due diligence actions the Commission's FAQ lists ([[official/faq_4-4-2]]), and documentation from the component's maker is the kind of evidence the guidance expects due diligence to rest on ([[CRA-GUIDANCE point 171]]).

An upstream SBOM describes the component as the project ships it, not as it sits in your product. Your build typically includes part of it, with your configuration, your patches and the components you added, so a copy of the upstream document would over-report what you ship and miss what you changed. The usual way is to generate your product's SBOM from your own build and use the upstream SBOM to check and complete it.

Using it changes nothing about who is responsible for your product. For a component that is itself a CRA product, its manufacturer has to fix its vulnerabilities and you can rely on that, but keeping your product compliant, informing your users and shipping the update are still yours. For an open source component that was never placed on the market, and for a third-party component that is not subject to the CRA, because it was never placed on the EU market or was placed on it before the CRA applied, nobody else has obligations: its vulnerabilities in your product are yours to handle, with or without its supplier's help ([[official/faq_4-3-6]]; see [[manufacturers/dependencies]]). Many projects will have no SBOM to offer: an _open-source software steward_ is not required to provide one, and a project outside the CRA has no obligations at all ([[stewards/sbom]]). The CRA prescribes no SBOM format beyond _"a commonly used and machine-readable format"_; the Commission may specify one by implementing act ([[CRA Article 13(24)]]).
