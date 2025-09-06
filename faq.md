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

See [FAQ README][].

#### Maturity level of answers

See [FAQ README][].

## Frequently Asked Questions about the Cyber Resilience Act (CRA)

### The Cyber Resilience Act (CRA) itself

* [What is the Cyber Resilience Act (CRA)?](./faq/cra-itself/cra.md) <a name="q-what-is-the-cyber-resilience-act-cra"></a><a name="faq-tmp-154"></a>
* [Where is the official text of the CRA?](./faq/cra-itself/text.md) <a name="q-where-is-the-official-text-of-the-cra"></a><a name="faq-tmp-155"></a>
* [When does the CRA enter into force and when does the regulation start to apply?](./faq/cra-itself/timeline.md) <a name="q-when-does-the-cra-enter-into-force-and-when-does-the-regulation-start-to-apply"></a><a name="faq-tmp-10"></a>
* [What kinds of products are regulated by the CRA?](./faq/cra-itself/scope.md) <a name="q-what-is-in-scope-of-the-cra"></a><a name="faq-tmp-2"></a>
* [What kinds of products are NOT regulated by the CRA?](./faq/cra-itself/out-of-scope.md) <a name="q-what-is-not-in-scope-of-the-cra"></a><a name="faq-tmp-156"></a> 
* [What is the 'CE Mark' and do I need to add it to my software?](./faq/cra-itself/ce-mark.md) <a name="q-As-an-open-source-steward-do-i-have-to-affix-the-ce-mark"></a><a name="faq-tmp-34"></a> 


### Open source projects

* [What criteria determine whether an open source project is in scope of the CRA?](./faq/projects/scope.md) <a name="q-what-criteria-determine-whether-an-open-source-project-is-in-scope-of-the-cra"></a><a name="faq-tmp-124"></a>
* [What does "Monetizing without making a profit" mean?](./faq/projects/monetizing.md) <a name="q-what-is-monetizing"></a><a name="faq-tmp-33"></a>
* [What does "Monetizing without making a profit" mean?](./faq/projects/monetizing.md) <a name="q-is-distributing-binaries-or-container-images-of-an-open-source-project-considered-as-making-it-available-on-the-market"></a><a name="faq-tmp-157"></a>

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
- On the basis of [Recital 18][] of the Cyber Resilience Act, I do not fall within the scope of the regulation, and cannot be considered as a Manufacturer or an Open source software steward under the Cyber Resilience Act.
- On the basis of [PLD Recital 15][], I cannot be held liable for your use of my code.
- **While I don't have obligations towards you, you may have some towards me:**
	- On the basis of [Article 13(6)][] the Cyber Resilience Act, if you believe you have found a security flaw in this code, you are responsible for reporting it by following the vulnerability disclosure process here: << project link >>. You are also responsible for fixing it within your product and providing the fix upstream.
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

* [Do all open source projects have an _open source software steward_?](./faq/stewards/do-all-projects-have-stewards.md) <a name="faq-tmp-170"></a>
* [What is an _open-source software steward_?](./faq/stewards/what-is-a-steward.md) <a name="q-what-is-an-open-source-software-steward"></a><a name="faq-tmp-127"></a>
* [Who can be _open-source software steward_?](./faq/stewards/who-can-be-steward.md)
* [What are the obligations of _open-source software stewards_?](./faq/stewards/obligations.md) <a name="q-what-are-the-obligations-of-open-source-software-stewards"></a><a name="faq-tmp-159"></a> 
* [How do _open-source software stewards_ demonstrate that they meet their obligations?](./faq/stewards/demonstrate.md) <a name="q-how-do-open-source-software-stewards-demonstrate-that-they-meet-their-obligations"></a><a name="faq-tmp-11"></a> 
* [What happens when an _open-source software steward_ doesn't meet its obligations?](./faq/stewards/penalties.md) <a name="q-what-happens-when-an-open-source-software-steward-doesnt-meet-its-obligations"></a><a name="faq-tmp-158"></a> 
* [Does a steward bear the cost of translating and maintaining its policy documents in many of the EU languages?](./faq/stewards/translation-costs.md) <a name="q-does-a-steward-bear-translation-costs-into-many-languages"></a><a name="faq-tmp-152"></a> 

### Manufacturers

* [What is a _manufacturer_?](./faq/manufacturers/what-is-a-manufacturer.md) <a name="q-what-is-a-manufacturer"></a><a name="faq-tmp-59"></a> 
* [Can a _manufacturer_ also be an _open-source software steward_?](./faq/manufacturers/both-manufacturer-and-steward.md) <a name="q-can-a-manufacturer-also-be-an-open-source-software-steward"></a><a name="faq-tmp-30"></a> 

### Standards

* [What is a _harmonised standard_ and why does it matter?](./faq/standards/harmonised-standards.md) <a name="q-what-is-a-harmonized-standard-and-why-does-it-matter"></a><a name="faq-tmp-56"></a> 

### Important and Critical Product Categories

### Security attestations

* [What is a _security attestation_ in the CRA?](./faq/attestations/what-is-a-security-attestation.md) <a name="q-what-is-a-security-attestation-in-the-cra"></a><a name="faq-tmp-72"></a>

### EU Legislation

* [What is the _Blue Guide_?](./faq/legislation/blue-guide.md) <a name="q-what-is-the-blue-guide"></a><a name="faq-tmp-4"></a> 
* [What is the _New Legislative Framework_ (NLF)?](./faq/legislation/nlf.md) <a name="q-what-is-the-new-legislative-framework-nlf"></a><a name="faq-tmp-57"></a> 
* [What is a _legal person_?](./faq/legislation/legal-person.md) <a name="q-what-is-a-legal-person"></a><a name="faq-tmp-55"></a>

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
See [FAQ README][].

### Annex 2 - FAQ formats

See [FAQ README][].

[FAQ README]: ./faq/cra-itself/README.md

[benefit from guidance]: ./faq/cra-itself/README.md#questions-which-would-benefit-from-european-commission-guidance
[No answer yet]: ./faq/cra-itself/README.md#maturity-level
[Draft]: ./faq/cra-itself/README.md#maturity-level
[Pending review]: ./faq/cra-itself/README.md#maturity-level
[Pending guidance]: ./faq/cra-itself/README.md#maturity-level
[Approved]: ./faq/cra-itself/README.md#maturity-level

[CRA]: https://eur-lex.europa.eu/eli/reg/2024/2847/oj
[CRA HTML]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847
[Recital 15]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_15
[Recital 18]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_18
[Recital 19]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_19
[Recital 21]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_21
[Recital 120]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_120
[Recital 121]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#rct_121
[Article 3(13)]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_3
[Article 3(14)]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_3
[Article 13(6)]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_13
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
