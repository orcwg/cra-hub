---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/11
---

# Will open source stewards be expected to provide an SBOM?

No, open-source software stewards are not required to provide a Software Bill of Materials (SBOM). The CRA places SBOM obligations on manufacturers, not stewards.

SBOMs are most meaningful when created by manufacturers at the point of integration, since they are responsible for documenting the components contained in their products with digital elements ([[Recital 77]]). The manufacturer's SBOM reflects the specific components they have integrated and helps them track vulnerabilities throughout the supply chain.

However, stewards may choose to provide SBOMs voluntarily. This could be done as part of security attestations, alongside builds, or through other means that help downstream manufacturers exercise due diligence and produce their own SBOMs more easily. Such voluntary efforts can support the broader open source ecosystem without creating regulatory obligations for stewards.

For more on steward obligations, see [[stewards/obligations]].
