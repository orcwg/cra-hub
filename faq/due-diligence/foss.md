---
Status: ✅ Approved
Related issues: https://github.com/orcwg/cra-hub/issues/305, https://github.com/orcwg/cra-hub/issues/71
---

# What level of due diligence is reasonable for manufacturers integrating open source components?

The reasonable level of due diligence for an open source component depends on the nature and level of cybersecurity risk of that component, as for any other third-party component. The Commission's FAQ says so: _"the appropriate level of due diligence is dependent on the nature and level of cybersecurity risk of a given open-source component"_ ([[official/faq_4-4-4]], [[official/faq_4-4-2]]). You may integrate open source components outside the scope of the CRA, or published by an _open-source software steward_, as long as they do not compromise the cybersecurity of your product ([[official/faq_4-4-4]], [[CRA Article 13(5)]]).

What due diligence involves, and the actions [[CRA Recital 34]] lists to choose from, such as the component's security update history, known vulnerabilities in public databases and your own tests, is covered in [[due-diligence/what-is-due-diligence]] ([[official/faq_4-4-2]]). The Commission's guidance sums up the exercise as working out what your product needs from the component and verifying that it delivers it ([[CRA-GUIDANCE point 171]]).

If you find a vulnerability in the component, you have to report it to whoever maintains it, through the channels the project publishes, fix it in your product, and share any fix you develop with them ([[CRA Article 13(6)]], [[CRA-GUIDANCE point 223]], [[CRA-GUIDANCE point 226]]). A project with no contact address or no maintainer does not lower your obligations for your own product: the guidance says you need not report upstream _"where the component no longer has a maintainer"_, but should inform its users another way ([[CRA-GUIDANCE point 225]]), and the Commission's FAQ says that where the project is _"not supporting the manufacturer in addressing and remediating vulnerabilities"_, you address them yourself, by disabling the function, switching components or patching the component ([[official/faq_4-3-6]]).

The CRA also lets the Commission set up voluntary security attestation programmes for open source software, which the Commission's FAQ says _"would facilitate manufacturers' due diligence obligation"_ where available ([[CRA Article 25]], [[official/faq_4-4-4]]): see [[due-diligence/relation-to-attestations]].
