# CRA FAQ

## About this document

This document represents a community effort to collect and answer frequently asked questions about the Cyber Resilience Act (CRA) as it relates to open source. 

The purpose of this document is twofold:

1. to consolidate community understanding of the CRA, and
2. to outline areas of the CRA which remain unclear and would [benefit from guidance][] from the European Commission.

### Disclaimer

> [!WARNING]
> Nothing contained in this document constitutes legal advice. If you have any legal questions about the CRA, you should consult with an attorney.

### Document Status

This is a draft document and may be updated, replaced or obsoleted at any time. It is inappropriate to cite this document as other than a work in progress. Publication of this document as a draft does not imply endorsement by the Eclipse Foundation, Open Regulatory Working Group Members, or contributors.

### Issue tracker

Open issues, pull requests, and untriagged FAQs can be found on [GitHub](https://github.com/orcwg/cra-hub/labels/FAQ).

### Notation conventions

#### Questions which would benefit from European Commission guidance

Frequently asked questions which would benefit from guidance from the European Commission are indicated with the following callout:

**🛑 CAUTION:** Pending confirmation through European Commission Guidance that [REASON].

#### Maturity level of answers

The maturity level of the answers contained in this document are indicated using the following system:

| Maturity level status | Icon | Description |
| :-------------------- |:----:| :---------- |
| No answer yet         |   ❓  | No answer has been drafted yet. |
| Draft                 |   ⚠️  | Hasn't been reviewed by SIG. Answer may be incomplete or incorrect. |
| Pending Review        |   👀  | Ready to be reviewed by the SIG. |
| Pending Guidance      |   🛑  | Identified by the SIG as requiring input from the EU Commission. |
| Approved              |   ✅  | Has been reviewed by the SIG. Represents community best effort to provide an actionable answer. |

Maturity level statuses are assigned using the process described in [Annex 1](#annex-1) below.


## Frequently Asked Questions about the Cyber Resilience Act (CRA)

### The Cyber Resilience Act (CRA) itself

<details>
    <a name="q-what-is-the-cyber-resilience-act-cra"></a>
    <summary><strong><a name="faq-tmp-154" href="#faq-tmp-154">tmp-154.</a> What is the Cyber Resilience Act (CRA)?</strong></summary>

The Cyber Resilience Act (CRA) is a new EU Regulation that aims to safeguard consumers and businesses who use software or products with digital components. It creates mandatory cybersecurity requirements for manufacturers and retailers that extend throughout the product lifecycle and the whole software supply chain (including all open source dependencies and transitive dependencies) and helps consumers and business identify such products through the [CE mark](https://en.wikipedia.org/wiki/CE_marking).

> Status: ✅ [Approved][]
| GitHub issue(s): [#154](https://github.com/orcwg/cra-hub/issues/154)
</details>

<details>
    <a name="q-where-is-the-official-text-of-the-cra"></a>
    <summary><strong><a name="faq-tmp-155" href="#faq-tmp-155">tmp-155.</a> Where is the official text of the CRA?</strong></summary>

The final text of the CRA can be found on [EUR-Lex][CRA] ([English HTML version][CRA HTML]).

> Status: ✅ [Approved][]
| GitHub issue(s): [#155](https://github.com/orcwg/cra-hub/issues/155)
</details>


<details>
    <a name="q-when-does-the-cra-enter-into-force-and-when-does-the-regulation-start-to-apply"></a>
    <summary><strong><a name="faq-tmp-10" href="#faq-tmp-10">tmp-10.</a> When does the CRA enter into force and when does the regulation start to apply?</strong></summary>


The CRA enters into force on December 11, 2024. Reporting obligations of actively exploited vulnerabilities and severe incidents ([Article 14][]) start to apply on September 11, 2026.
All other obligations for software developers start to apply on December 11, 2027. _(Source: [Article 71][])_

```mermaid
%%{init: {'theme':'base'}}%%
gantt
    title CRA Implementation Timeline
    dateFormat  YYYY-MM-DD
    axisFormat %Y-Q%q
    tickInterval 3month

    Drafting phase: 2024-01-01, 2024-11-20
    Publication in the Official Journal of the EU (November 20, 2024): milestone, 2024-11-20, 5m
    Entry into force (December 11, 2024): milestone, 2024-12-11, 5m
    Implementation phase: 2024-12-11, 3y
    Reporting obligations of vulnerabilities and incidents (September 11, 2026): milestone, 2026-09-11, 5m
    Notification of conformity of assessment bodies (June 11, 2026): milestone, 2027-06-11, 5m
    All other obligations (December 11, 2027): milestone, 2027-12-11, 5m
    Application phase: 2026-09-11, 2029-06-30
```

> Status: ✅ [Approved][]
| GitHub issue(s): [#10](https://github.com/orcwg/cra-hub/issues/10)
</details>


<details>
    <a name="q-what-is-in-scope-of-the-cra"></a>
    <summary><strong><a name="faq-tmp-2" href="#faq-tmp-2">tmp-2.</a> What kinds of products are regulated by the CRA?</strong></summary>

The following types of product are "in scope" (i.e., their design and production may be regulated by) the CRA:

- Hardware products (e.g. laptops, smart appliances, mobile phones, network equipment, CPUs, etc.)
- Software products (e.g. operating systems, word processing, games or mobile apps, software libraries, etc.)
- Remote data processing solutions for any of the above, as far as those solutions are necessary for a product to perform its functions (e.g. cloud-based services that allow control of a smart lock at a distance, remote database that backs-up user preferences, etc.)

> Status: ✅ [Approved][]
| GitHub issue(s): [#2](https://github.com/orcwg/cra-hub/issues/2)
</details>


<details>
    <a name="q-As-an-open-source-steward-do-i-have-to-affix-the-ce-mark"></a>
    <summary><strong><a name="faq-tmp-34" href="#faq-tmp-34">tmp-34.</a> What is the 'CE Mark' and do I need to add it to my software ?</em></strong></summary>
The CE mark is a distinctive symbol indicating that a product complies with the relevant EU product regulations. <strong>Under the CRA, only manufacturers are authorized to affix the CE mark to a product.</strong> Open Source software stewards, and developers outside the scope of the law cannot do so

For Manufacturers, under the Cyber Resilience Act (CRA), Article 30 of the Regulation outlines the requirements for CE marking on digital products, whether hardware or software.
- Hardware: The CE mark must, in principle, be affixed directly to the product. If this is not feasible, it may be placed on the packaging and in the EU declaration of conformity.
- Software: The CE mark must appear either in the EU declaration of conformity or on a website accompanying the software product, provided it is easily accessible to consumers.

Failure to properly affix the CE mark when required may result in financial penalties, as defined by national law.

> Status:✅ [Approved][]
| GitHub issue(s): [#34](https://github.com/orcwg/cra-hub/issues/34)
</details>


<details>
    <a name="q-what-is-not-in-scope-of-the-cra"></a>
    <summary><strong><a name="faq-tmp-156" href="#faq-tmp-156">tmp-156.</a> What is NOT in scope of the CRA?</strong></summary>

The following types of product are NOT in scope of the CRA:

- Products already covered by other regulations or directives: civil aviation equipment ([2018/1139][]), marine equipment ([2014/90][]), medical devices ([2017/745][] and [2017/746][]), motor vehicles ([2019/2144][]), and software as a service (SaaS) ([NIS 2][])
- Products exclusively designed for national security or defence purposes
- Products specifically designed to process classified information

_It is worth noting however, that the intent of the EU legislators is to harmonize the various regulations mentioned above with the CRA in the near future._

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#156](https://github.com/orcwg/cra-hub/issues/156)
</details>


### Open source projects

<details>
    <a name="q-what-criteria-determine-whether-an-open-source-project-is-in-scope-of-the-cra"></a>
    <summary><strong><a name="faq-tmp-124" href="#faq-tmp-124">tmp-124.</a> What criteria determine whether an open source project is in scope of the CRA?</strong></summary>

The CRA regulates _natural and legal persons_ (either an individual or an organisation that has a legal personality, like a business, foundation or charity). There are three possible categories with descending requirements. These categories are _manufacturer_, _Open Source Software Steward_, or _Out of Scope_.
> Note: At present, we believe that a natural person (an individual) cannot be considered an Open Source Software Steward, however we are currently verifying this with the European Commission. We will provide more detailed guidance as soon as possible.

- You are **out of scope** of the CRA (meaning you are not required to comply with the regulation), if you are a natural person (an individual), and:
  - you are not monetising your project at all, or
  - you are monetising your project, without the intention of making a profit. (See Question: What does "Monetizing without making a profit" mean?)

> Note: Further information for legal persons (organisations, foundations, associations) will be provided here as soon as we receive further clarifications and information from the European Commission.
> Status: ❓ [No answer yet][]
| GitHub issue(s): [#124](https://github.com/orcwg/cra-hub/issues/124)
</details>


<details>
    <a name="q-what-is-monetizing"></a>
    <summary><strong><a name="faq-tmp-33" href="#faq-tmp-33">tmp-33.</a> What does "Monetizing without making a profit" mean?</strong></summary>
	
- As an individual, if you are monetizing your project without the intention of making a profit, you are outside the scope of the regulation.
- According to [Recital 15 of the CRA](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_15), monetising without intention of making a profit means you fulfil the following cumulative requirements:
    - You are not providing a software platform through which you monetise other services (for instance, Google's Android).
    - You are not requiring as a condition for use the processing of personal data for reasons other than exclusively for improving the security, compatibility or interoperability of your software. (in particular, you're not giving people access to your software in exchange for their personal data)
   - You are receiving donations or providing technical services in exchange for remuneration, where the total received does not exceed the cost of development of your software (hosting, hardware, compute etc..).

> Note: We are waiting for clarification from the Commission as to if remuneration for hours worked on the project can be counted in the cost of development. 
> Status: 🛑 [Pending Guidance][]
| GitHub issue(s): [#33](https://github.com/orcwg/cra-hub/issues/33)
</details>


<details>
    <a name="q-is-distributing-binaries-or-container-images-of-an-open-source-project-considered-as-making-it-available-on-the-market"></a>
    <summary><strong><a name="faq-tmp-157" href="#faq-tmp-157">tmp-157.</a> Is distributing binaries or container images of an open source project considered as making it available on the market?</strong></summary>

No. Monetization by the original manufacturer is what determines whether a product is made available on the market. As per [Recital 18][], merely supplying open source components isn't indicative of a commercial activity:

> Furthermore, the supply of products with digital elements qualifying as free and open-source software components intended for integration by other manufacturers into their own products with digital elements should be considered to be making available on the market only if the component is monetised by its original manufacturer. […] In addition, the mere presence of regular releases should not in itself lead to the conclusion that a product with digital elements is supplied in the course of a commercial activity.

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#157](https://github.com/orcwg/cra-hub/issues/157)
</details>


### Maintainers

<details>
    <a name="q-should-i-worry-about-the-CRA"></a>
    <summary><strong><a name="faq-tmp-133a" href="#faq-tmp-133a">tmp-133a.</a> I am worried about how the CRA might impact me, and so I am considering shutting down my open source projects. Should I do that?</strong></summary>

The CRA should have zero or minimal impact on most open source developers, so you should probably not shut down your open source projects because of the CRA. There are several reasons for this:

First, the CRA likely does not apply to you. 

- If you're just a contributor, the CRA explicitly exempts you. For more detail, see [tmp-17](#faq-tmp-17).
- If you're a maintainer, and you _do not_ "monetise" your FOSS codebase, the CRA explicitly exempts you. For more detail, see [tmp-133b](#faq-tmp-133b).
- If you're a maintainer, and you _do_ monetise your FOSS codebase, you may still be exempted, depending on exactly how you are monetizing the codebase and your participation in it. For more detail, see [tmp-133c](#faq-tmp-133c).

Second, even if the CRA does ultimately apply to you, penalties for solo and small-team maintainers are unlikely to be severe. For more detail, see [tmp-133d](#faq-tmp-133d).

As a result, we would strongly urge you _not_ to shut down any open source projects (or your participation in those projects) just because of the CRA.

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#133](https://github.com/orcwg/cra-hub/issues/133)
</details>

<details>
    <a name="q-am-i-subject-to-the-cra-if-i-only-contribute-to-an-open-source-project"></a>
    <summary><strong><a name="faq-tmp-17" href="#faq-tmp-17">tmp-17.</a> Am I subject to the CRA if I only contribute to an open source project?</strong></summary>

No. Contributions to an open source codebase are explicitely not in scope of the CRA. See [Recital 18][]: 

> This Regulation does not apply to natural or legal persons who contribute with source code to products with digital elements qualifying as free and open-source software that are not under their responsibility.

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#17](https://github.com/orcwg/cra-hub/issues/17)
</details>

<details>
    <a name="q-am-I-subject-if-I-dont-monetise"></a>
    <summary><strong><a name="faq-tmp-133b" href="#faq-tmp-133b">tmp-133b.</a> Am I subject to the CRA if I maintain, but do not monetise, an open source project?</strong></summary>

If you are the maintainer of an open source codebase, and you do not monetise it, then the CRA _does not_ require you to do _anything_.

The CRA applies
> only in relation to products... supplied ... in the course of a _commercial activity_
([Recital 15][], emphasis added)

And it states that

> the provision of ... free and open-source software that are not monetised by their manufacturers _should not be considered to be a commercial activity_
([Recital 18][], emphasis added)


> Status: ⚠️ [Draft][]
| GitHub issue(s): [#133](https://github.com/orcwg/cra-hub/issues/133)
</details>

<details>
    <a name="q-am-I-subject-if-I-do-monetise"></a>
    <summary><strong><a name="faq-tmp-133c" href="#faq-tmp-133c">tmp-133c.</a> Am I subject to the CRA if I maintain and monetise an open source project?</strong></summary>

If you are the maintainer of an open source codebase, and you do monetise it, then the CRA may apply to you, since you may be participating in a "commercial activity". 

However, there are at least two significant exceptions that may allow you to take money for your work without being subject to the CRA.

- If you monetise your software only by accepting donations that cover the "costs associated with the design, development, and provision" of the product, then the CRA says your participation is not a "commercial activity" and so it does not regulate you or your codebase. (See [Recital 15][] for more details.)
- If you monetise your software by charging for a security attestation programme, that may also not be a "commercial activity" for purposes of the regulation. The exact nature of that exemption is still to be determined. (See [Recital 21][] for more details.)

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#133](https://github.com/orcwg/cra-hub/issues/133)
</details>

<details>
    <a name="q-what-penalties"></a>
    <summary><strong><a name="faq-tmp-133d" href="#faq-tmp-133d">tmp-133d.</a> If I maintain an open source codebase, and am treated as a "manufacturer" or "steward", what penalties could I face for violating the CRA?</strong></summary>

If you are a solo or small-team maintainer of an open source codebase, but do get treated as a manufacturer or steward for some reason (such as [monetisation](#faq-tmp-133c)), you may be subject to some penalties. However, the penalties should be limited. In particular:

- If you are regulated because you are a steward, stewards are explicitly exempted from any fines, though you may still be required to take corrective actions for any problems that are uncovered. See [Article 64][].

- If you are regulated because you are a manufacturer, penalties must still be constrained. Specifically, all penalties must be "proportionate" ([Recital 120][]; [Article 64][]). In addition, when imposed on a natural person, the penalties must take into account "the economic situation" and "size" of the entity ([Recital 121]; [Article 64][]). As a result, while it is not formally required, most regulators will likely to request corrective action before imposing a fine.

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#133](https://github.com/orcwg/cra-hub/issues/133)
</details>

<details>
    <summary><strong><a name="faq-tmp-70" href="#faq-tmp-70">tmp-70.</a> I am NOT subject to the CRA, and want to make this clear to downstream users. What should I say?</strong></summary>
  
Reply to their requests, stating the following:
<code>
- On the basis of [Recital 18 of the Cyber Resilience Act](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_18), I do not fall within the scope of the regulation, and cannot be considered as a Manufacturer or an Open source software steward under the Cyber Resilience Act.
- On the basis of [Recital 15 of the Product Liability Directive](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402853#rct_15), I cannot be held liable for your use of my code.
- **While I don't have obligations towards you, you may have some towards me:**
	- On the basis of [Article 13.6 the Cyber Resilience Act](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_13), if you believe you have found a security flaw in this code, you are responsible for reporting it by following the vulnerability disclosure process here: << project link >>. You are also responsible for fixing it within your product and providing the fix upstream.
</code>

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#70](https://github.com/orcwg/cra-hub/issues/70)
</details>


<details>
    <a name="q-can-an-solo-maintainer-be-considered-to-be-an-open-source-software-steward"></a>
    <summary><strong><a name="faq-tmp-1" href="#faq-tmp-1">tmp-1.</a> Can an solo maintainer be considered to be an <em>open-source software steward</em>?</strong></summary>

No. As defined in [Article 3(14)][], an _open-source software steward_ must be a _legal person_ (e.g. a company, an organization, etc.) in contrast with a _natural person_ (i.e. a human being). The obligations of _open-source software stewards_ described in [Article 24][] therefore do not apply to solo maintainers. It is worth noting however, that _natural persons_ are subject to the same obligations as _legal persons_ would be should they monetize their poject.

**🛑 CAUTION:** Pending confirmation through European Commission Guidance that _legal persons_ do not include _natural persons_ in the context of the CRA.

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#1](https://github.com/orcwg/cra-hub/issues/1)
</details>


<details>
    <a name="q-can-a-loosely-organized-group-of-maintainers-be-considered-to-be-an-open-source-software-steward"></a>
    <summary><strong><a name="faq-tmp-15" href="#faq-tmp-15">tmp-15.</a> Can a loosely organized group of maintainers be considered to be an <em>open-source software steward</em>?</strong></summary>

No. As defined in [Article 3(14)][], an _open-source software steward_ must be a _legal person_, which in the context of the CRA means an legal entity such as a business or nonprofit.

**🛑 CAUTION:** Pending confirmation through European Commission Guidance that _legal persons_ do not include _natural persons_ in the context of the CRA.

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#15](https://github.com/orcwg/cra-hub/issues/15)
</details>


### Open-Source Software Stewards


<details>
    <summary><strong><a name="faq-tmp-170" href="#faq-tmp-170">tmp-170.</a> Do all open source projects have an <em>open source software steward</em>?</strong></summary>

No. Most open source projects will not have a steward. 

A steward must be a "legal person" (Art. 3), such as a company, and most open source projects are not supported by a company. 

The stewarding organization must also have "the purpose or objective of systematically providing support on a sustained basis" (Art. 3) and their software must be "ultimately intended for commercial activities" (recital 19). Organizations who do not meet those tests will also not be considered stewards.

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#170](https://github.com/orcwg/cra-hub/issues/170)
</details>


<details>
    <a name="q-what-is-an-open-source-software-steward"></a>
    <summary><strong><a name="faq-tmp-127" href="#faq-tmp-127">tmp-127.</a> What is an <em>open-source software steward</em>?</strong></summary>

_Open-source software steward_ is a term defined in [Article 3(14)][] of the CRA, to subject specific organisations to a subset of CRA obligations because they exist to support free and open source software that is intended for commercial activities (by others):

> ‘open-source software steward’ means a legal person, other than a manufacturer, that has the purpose or objective of systematically providing support on a sustained basis for the development of specific products with digital elements, qualifying as free and open-source software and intended for commercial activities, and that ensures the viability of those products;

[Recital 19][] states "Open-source software stewards include certain foundations as well as entities that develop and publish free and open-source software in a business context, including not-for-profit entities." At [FOSDEM 2024][FOSDEM24], the European Commission provided three examples of entities the co-legislators had in mind [^EC@FOSDEM24]:

  1. Foundations supporting specific FOSS projects
  2. Companies that build FOSS for their own use but make it public
  3. Not-for-profit entities that develop FOSS

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#127](https://github.com/orcwg/cra-hub/issues/127)
</details>


<details>
    <a name="q-what-are-the-obligations-of-open-source-software-stewards"></a>
    <summary><strong><a name="faq-tmp-159" href="#faq-tmp-159">tmp-159.</a> What are the obligations of <em>open-source software stewards</em>?</strong></summary>

_Open-source software stewards_ are subject to a "light-touch and tailor-made regulatory regime" ([Recital 19][]), defined in [Article 24][].

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#159](https://github.com/orcwg/cra-hub/issues/159)
</details>

<details>
    <a name="q-how-do-open-source-software-stewards-demonstrate-that-they-meet-their-obligations"></a>
    <summary><strong><a name="faq-tmp-11" href="#faq-tmp-11">tmp-11.</a> How do <em>open-source software stewards</em> demonstrate that they meet their obligations?</strong></summary>

> Status: ❓ [No answer yet][]
| GitHub issue(s): [#11](https://github.com/orcwg/cra-hub/issues/11)
</details>


<details>
    <a name="q-what-happens-when-an-open-source-software-steward-doesnt-meet-its-obligations"></a>
    <summary><strong><a name="faq-tmp-158" href="#faq-tmp-158">tmp-158.</a> What happens when an <em>open-source software steward</em> doesn't meet its obligations?</strong></summary>

> Status: ❓ [No answer yet][]
| GitHub issue(s): [#158](https://github.com/orcwg/cra-hub/issues/158)
</details>

<details>
	<a name="q-does-a-steward-bear-translation-costs-into-many-languages"></a>
	<summary><strong><a name="faq-tmp-152" href="#faq-tmp-152">tmp-152.</a> Does a steward bear the cost of translating and maintain its policy documents in many of the EU languages?</strong></summary>

> Status: 🛑 [Pending Guidance][]
| GitHub issue(s): [#152](https://github.com/orcwg/cra-hub/issues/152)
</details>


### Manufacturers

<details>
    <a name="q-what-is-a-manufacturer"></a>
	<summary><strong><a name="faq-tmp-59" href="#faq-tmp-59">tmp-59.</a> What is a <em>manufacturer</em>?</strong></summary>

The term _Manufacturer_ is defined in [Article 3(13)][] of the CRA:
	
> ‘manufacturer’ means a natural or legal person who develops or manufactures products with digital elements or has products with digital elements designed, developed or manufactured, and markets them under its name or trademark, whether for payment, monetisation or free of charge;

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#59](https://github.com/orcwg/cra-hub/issues/59)
</details>


<details>
	<a name="q-can-a-manufacturer-also-be-an-open-source-software-steward"></a>
	<summary><strong><a name="faq-tmp-30" href="#faq-tmp-30">tmp-30.</a> Can a <em>manufacturer</em> also be an <em>open-source software steward</em>?</strong></summary>

Yes, a _manufacturer_ can also be an _open-source software steward_, but it cannot be both the _manufacturer_ and _open-source software steward_ of the same project.

In 2024 Benjamin Bögel of the European Commission gave a FOSDEM presentation and specifically gave, as examples of stewards, “companies that build [OSS] for their use [for integration into their own products] but make [the OSS] public.” [^EC@FOSDEM24][]. This only makes sense if an organization can be a manufacturer for one program and a steward for another.

Mike Bursell, Co-chair, OpenSSF Cyber Policy Working Group (WG), believes that “if the organisation both sells a PDE that uses [some] open source project, and [separately] hosts [that open source project], supports it, and provides updates and patches for the community [that’s a real community]… then that would put [the organization] in both categories [depending on which software is being discussed].” [Bursell2025][]

Whether or not an organization is a steward depends on many specifics. If the organization meets the criteria for a _manufacturer_ for some software, by definition it is a _manufacturer_. For more information, see CRA [Recital 18][] and the [PLD Recital 15]().

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#30](https://github.com/orcwg/cra-hub/issues/30)
</details>


### Standards

<details>
    <a name="q-what-is-a-harmonized-standard-and-why-does-it-matter"></a>
    <summary><strong><a name="faq-tmp-56" href="#faq-tmp-56">tmp-56.</a> What is a <em>harmonised standard</em> and why does it matter?</strong></summary>

A _harmonised standard_ is a standard adopted by one of the [European Standardisation Organisations (ESOs)][ESO].
Certain (but not all) _harmonised standards_ are referenced in the [_Official Journal of the European Union_][OJEU] by the European Commission.
Harmonised standards referenced in this way provide products that conform with them a _presumption of conformity_ with the requirements covered by those standards.
Harmonised standards may be referenced with restrictions, in which case they only provide partial _presumption of conformity_.
The _presumption of conformity_ provided by harmonised standards referenced in the _Official Journal of the European Union_ is why it is expected that most organisations will choose to implement such standards when they exist, to comply with the CRA.

However, not all harmonised standards are referenced.
Those that are not referenced are often foundational standards upon which other standards build. In general, only the vertical (product-specific) standards are referenced, though sometimes horizontal standards that cover generic requirements may be referenced with restrictions.

The ORC WG maintains a [list of _harmonised standards_][standards] requested by the European Commission to the ESOs.
  
> Status: ⚠️ [Draft][]
| GitHub issue(s): [#56](https://github.com/orcwg/cra-hub/issues/56)
</details>

### Important and Critical Product Categories

### EU Legislation

<details>
	<a name="q-what-is-the-blue-guide"></a>
	<summary><strong><a name="faq-tmp-4" href="#faq-tmp-4">tmp-4.</a> What is the <em>Blue Guide</em>?</strong></summary>

The [Blue Guide][] is one of the main reference documents of the European Commission explaining how to implement legislation based on the New Legislative Framework (NLF). Unlike the CRA, the Blue Guide does not have legal force. It predates the CRA and only discusses software as something embedded into a physical product, not as standalone.
For this reason, until an updated version is available, the Blue Guide's guidance should be read in light of the CRA's wider scope and take into account the nuances introduced in the CRA for software. For example, on the concept of "commercial activity", [Recital 18][] CRA provides more specific guidance on "monetisation" and "non-profit organisations" than is available in the Blue Guide's "Making available on the market" section.

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#4](https://github.com/orcwg/cra-hub/issues/4)
</details>


<details>
    <a name="q-what-is-the-new-legislative-framework-nlf"></a>
    <summary><strong><a name="faq-tmp-57" href="#faq-tmp-57">tmp-57.</a> What is the <em>New Legislative Framework</em> (NLF)?</strong></summary>	

> Status: ❓ [No answer yet][]
| GitHub issue(s): [#56](https://github.com/orcwg/cra-hub/issues/56)
</details>


<details>
	<a name="q-what-is-a-legal-person"></a>
	<summary><strong><a name="faq-tmp-55" href="#faq-tmp-55">tmp-55.</a> What is a <em>legal person</em>?</strong></summary>

In the context of the CRA, a _legal person_ means an legal entity such as a business or nonprofit.

**🛑 CAUTION:** Pending confirmation through European Commission Guidance that _legal persons_ do not include _natural persons_ in the context of the CRA.

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#55](https://github.com/orcwg/cra-hub/issues/55)
</details>

<details>
    <a name="q-what-is-a-security-attestation-in-the-cra"></a>
    <summary><strong><a name="faq-tmp-72" href="#faq-tmp-72">tmp-72.</a> What is a <em>security attestation</em> in the CRA?</strong></summary>

Security attestations in the CRA are an optional extension that do not exist yet. They may exist in the future, should the European Commission choose to establish them, with a legislative process called a "delegated act". Until such time, any resemblence with concepts elsewhere by the name of "attestation" is coincidental and should not restrict their future design in the CRA. For example, the "Secure Software Development Attestation" as a concept in the US is unrelated to the CRA.

> Status: ⚠️ [Draft][]
| GitHub issue(s): [#72](https://github.com/orcwg/cra-hub/issues/72)
</details>

## Acknowledgments

The following people have contributed to this document either directly or indirectly (e.g. by raising questions):
Adrian O'Sullivan,
Aeva Black,
Alberto Pianon,
Alex Lennon,
Alistair Woodman,
Chris Jenkins,
Christopher "CRob" Robinson,
Daniel Appelquist,
Daniel Stenberg,
Dick Brooks,
Dirk-Willem van Gulik,
Felix Reda,
Florian Idelberger,
Gesine Freund,
Hermann Seuschek,
Ilonka Sievers,
Jakub Zelenka,
Jan Westerkamp,
John Ellis,
Jordan Maris,
Juan Rico,
Lars Francke,
Luis Villa,
Maarten Aertsen,
Marta Rybczynska,
Mattias Dahlberg,
Maxim Baele,
Mikaël Barbero,
Mike Bursell,
Nils Adermann,
Olle E. Johansson,
Pete Allor,
Piotr P. Karwasz,
Poul-Henning Kamp,
Ria Schalnat,
Roman Zhukov,
Ruth Suehle,
Salve J. Nilsen,
Seth Michael Larson,
Simon Phipps,
Stefane Fermigier,
Timo Perala,
Timothée Mazzucotelli,
Tobie Langel,
and Victor Roland.

If you have contributed to this document and aren't properly acknowledged or if you want to edit or remove your name, please let us know by [opening an issue](https://github.com/orcwg/cra-hub/issues/new) and we will fix this right away.

## Annexes

### Annex 1 - Maturity level process

<a name="annex-1"></a>
Maturity level statuses are assigned using the following process. All answers start with a maturity level status of "No answer yet".

```mermaid
flowchart TD
    start[Status: No answer yet ❓]
    A[Status: Draft ⚠️]
    B[Status: Pending Review 👀]
    C[Status: Approved ✅]
    D[Status: Pending Guidance 🛑]
    start -- Add draft answer --> A
    A -- Ready for review --> B
    B --> SIG{"Passes SIG Review?"}
    SIG -- YES --> Q{"Requires EU guidance?"}
    SIG -- NO --> A
    Q -- NO --> C
    Q -- YES --> D
    D -- Guidance received --> SIG
```

### Annex 2 - FAQ formats

#### Draft FAQ format

```md
<details>
    <a name="PREVIOUS_ANCHOR_SO_WE_DONT_BREAK_EXTERNAL_REFERENCES"></a>
    <summary><strong><a name="faq-tmp-GITHUB_ISSUE_ID" href="#faq-tmp-GITHUB_ISSUE_ID">tmp-GITHUB_ISSUE_ID.</a> QUESTION</strong></summary>

ANSWER

> Status: ICON [MATURITY_LEVEL][]
| GitHub issue(s): [#GITHUB_ISSUE_ID](https://github.com/orcwg/cra-hub/issues/GITHUB_ISSUE_ID)
</details>
```

#### Final FAQ format

```md
<details>
    <a name="PREVIOUS_ANCHOR_SO_WE_DONT_BREAK_EXTERNAL_REFERENCES"></a>
    <a name="faq-tmp-GITHUB_ISSUE_ID"></a>
    <summary><strong><a name="faq-FINAL_ID" href="#faq-FINAL_ID">FINAL_ID.</a> QUESTION</strong></summary>

ANSWER

</details>
```

[benefit from guidance]: #questions-which-would-benefit-from-european-commission-guidance
[No answer yet]: #maturity-level-of-answers
[Draft]: #maturity-level-of-answers
[Pending review]: #maturity-level-of-answers
[Pending guidance]: #maturity-level-of-answers
[Approved]: #maturity-level-of-answers

[CRA]: https://eur-lex.europa.eu/eli/reg/2024/2847/oj
[CRA HTML]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847
[Recital 15]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_18
[Recital 18]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_18
[Recital 19]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_19
[Article 3(13)]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_3
[Article 3(14)]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_3
[Article 14]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_14
[Article 18]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_18
[Article 24]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_24
[Article 64(10)(b)]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_64
[Article 71]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_71
[Chapter IV]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#cpt_IV

[2014/90]: https://eur-lex.europa.eu/eli/dir/2014/90/oj
[2017/745]: https://eur-lex.europa.eu/eli/reg/2017/745/oj
[2017/746]: https://eur-lex.europa.eu/eli/reg/2017/746/oj
[2018/1139]: https://eur-lex.europa.eu/eli/reg/2018/1139/oj
[2019/2144]: https://eur-lex.europa.eu/eli/reg/2019/2144/oj
[NIS 2]: https://eur-lex.europa.eu/eli/dir/2022/2555/oj

[Blue Guide]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=CELEX:52022XC0629(04)
[ESO]: https://single-market-economy.ec.europa.eu/single-market/european-standards_en
[standards]: https://github.com/orcwg/cra-hub/blob/main/standards.md
[OJEU]: https://eur-lex.europa.eu/oj/direct-access.html 

[PLD Recital 15]: https://eur-lex.europa.eu/eli/dir/2024/2853#rct_15

[Bursell2024]: https://openssf.org/blog/2025/02/20/does-the-eu-cra-affect-my-business]

[^EC@FOSDEM24]: https://fosdem.org/2024/schedule/event/fosdem-2024-3683-the-regulators-are-coming-one-year-on/, at 18 min 10 seconds into the recording
