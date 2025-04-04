# Inventory of resources relevant to the horizontal CRA standards, Open Source Steward obligations, and voluntary attestation program

The goal of this document is to collect resources that are relevant to the CRA obligations of _open-source software stewards_ and _manufacturers_ when it comes to the development and usage of open source.

_Please add all relevant resources as a table row under the relevant section or subsection._

> [!Note]
> Additional resources are currently collected in this [spreadsheet](https://docs.google.com/spreadsheets/d/1Y36Vueb3Eo_djOuRdpyzoCS1vzGaKpjP-99g3J6rw7Y/edit?gid=0#gid=0) and will be folded into this document shortly.

## Table of Content

* [Principles of Cyber Resilience](#horizontal-type-a-standards-due-august-30-2026)
* [Horizontal Type B Standards (due Sept. 2027)](#horizontal-type-b-standards-due-october-30-2027)
* [Open Source Steward Cybersecurity policy](#open-source-steward-cybersecurity-policy)
* [Due diligence requirements of manufacturers](#due-diligence-requirements-of-manufacturers)
* [Voluntary security attestation programmes](#voluntary-security-attestation-programmes)
* [Other](#other)

## Principles of Cyber Resilience

> Designing, developing and producing products with digital elements in such a way that they ensure an appropriate level of cybersecurity based on the risks.

CRA ref: [Annex I, Part I, point (1)][Annex I]\
Standards request ref: [1](https://github.com/orcwg/cra-hub/blob/main/standards.md#milestone-1---horizontal-standards-due-august-30-2026)\
Impact on steward: `Partial obligation` ("foster development of secure product", [Article 24(1)][Article 24])

### Risk analysis

* [OWASP Software Assurance Maturity Model (SAMM)](https://owaspsamm.org), OWASP, CC-BY-SA-4.0, Maturity Model, 2009 – present. SAMM is a maturity model that helps organizations implement a Secure Development Lifecycle.

### Secure design & secure coding principles

* [OpenStack Secure Development Guidelines](https://security.openstack.org/#secure-development-guidelines), OpenStack Community, CC-BY-3.0, informal, 2015-02-18 – present.
* [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org), OWASP, CC BY-SA 4.0, Informal Guidelines, 2014 – present. OWASP Cheat Sheets are a collection of pragmatic security guidelines and best practices for a wide range of technologies.

### Security processes & governance

* [OWASP DevSecOps Maturity Model (DSOMM)](https://dsomm.owasp.org), OWASP, GPL-3, Maturity Model, 2017 – present. DSOMM is a maturity model aimed at implementing DevSecOps best practices.
* [NIST Secure Software Development Framework (NIST SP 800-218)](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-218.pdf), National Institute of Standards and Technology (NIST), No License Required, Guidelines, 2022-02 – present. SSDF is a set of community-derived and regulatory-aligned practices for the creation and usage of software.




### Designing, developing and producing products with digital elements in such a way that they ensure an appropriate level of cybersecurity based on the risks

CRA ref: [Annex I, Part I, point (1)][Annex I]\
Standards request ref: 1\
Impact on steward: `Partial obligation` ("foster development of secure product", [Article 24(1)][Article 24])


| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| [OpenStack Secure Development Guidelines](https://security.openstack.org/#secure-development-guidelines) | OpenStack Community | CC-BY-3.0 | informal | 2015-02-18 – present | |
| [OWASP Software Assurance Maturity Model (SAMM)](https://owaspsamm.org) | OWASP | CC-BY-SA-4.0 | Maturity Model | 2009 – present | SAMM is a maturity model that helps organizations implement a Secure Development Lifecycle. |
| [OWASP DevSecOps Maturity Model (DSOMM)](https://dsomm.owasp.org) | OWASP | GPL-3 | Maturity Model | 2017 – present | DSOMM is a maturity model aimed at implementing DevSecOps best practices. |
| [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org) | OWASP | CC BY-SA 4.0 | Informal Guidelines | 2014 – present | OWASP Cheat Sheets are a collection of pragmatic secruity guidelines and best practices for a wide range of technologies. |
| [NIST Secure Software Development Framework (NIST SP 800-218)](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-218.pdf) | National Institute of Standards and Technology (NIST) | No License Required | Guidelines | 2022-02 - present | SSDF is a set of community-derived and regulatory-aligned practices for the creation and usage of software |

### Vulnerability handling for products with digital elements

CRA ref: [Annex I, Part II][Annex I]\
Standards request ref: 15\
Impact on steward: `obligation`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| [OpenStack Vulnerability Management Process](https://security.openstack.org/vmt-process.html) | OpenStack Community | CC-BY-3.0 | informal | 2011-10-25 – present | Subsequently adapted by many other communities and early inspiration for standards like those compiled by CII/OpenSSF |
| [PHP Security Policies and Process](https://github.com/php/policies/blob/main/security-policies.rst) | PHP Project | none but [CC-BY-4.0 proposed](https://github.com/php/policies/blob/main/security-policies.rst) | informal | 2024-02-06 – present | Just initial info about managing security.txt file but it should contain more info in the future |
| [PHP Vulnerability Disclosure Policy](https://github.com/php/policies/blob/main/security-classification.rst) | PHP Project | none but [CC-BY-4.0 proposed](https://github.com/php/policies/blob/main/security-policies.rst) | informal | 2023-12-04 – present | Security issues classification and their handling |
| [RFC 9116](https://www.rfc-editor.org/rfc/rfc9116) | IETF | IETF Trust Legal Provisions (TLP) | RFC | 2022-04 | A File Format to Aid in Security Vulnerability Disclosure |
| [PHP release process](https://github.com/php/php-src/blob/master/docs/release-process.md) | PHP project | PHP 3.01 | informal | 2007-11-22 - present | It includes some info about releasing of security fixes |
| [ASF Classification of vulnerabilties ](https://security.apache.org/blog/severityrating/) | ASF | [ASLv2](https://www.apache.org/licenses/LICENSE-2.0) | practice | 25 Apr, 2023  | Captures lessons learned and best practices around vulnerability classification; Improves upon similar scales used by [Microsoft](https://www.microsoft.com/en-us/msrc/security-update-severity-rating-system?oneroute=true), OpenSSL, Red Hat various Apache projects] |
| [Generic ASF vulnerability reporting process](https://apache.org/security/) | ASF | [ASLv2](https://www.apache.org/licenses/LICENSE-2.0) | policy | current | Generic process for reporting a vulnerability (i.e. not project specific) |
|[Generic ASF handling process for vulnerabilities](https://apache.org/security/committers.html) | ASF | [ASLv2](https://www.apache.org/licenses/LICENSE-2.0) | policy | current | Generic process for developers to follow when handling a vulnerability report (i.e. not project/risk specific) |
| [Guide to coordinated vulnerability disclosure for open source software projects](https://github.com/ossf/oss-vulnerability-guide) | OpenSSF | CC-BY-4.0 | Guidance, templates, and advise for how open source projects and security researchers can better coordinate vulnerability disclosures together | 2022 - present | |
| [Guidelines and Practices for Multi-Party Vulnerability Coordination and Disclosure](https://www.first.org/global/sigs/vulnerability-coordination/multiparty/guidelines-v1.1) | Forum of Incident Response and Security Teams (FIRST) | none | Guidelines for handling coordiantion of complex (multiparty) vulnerabilities | Spring 2020 | |
| [The CERT® Guide to Coordinated Vulnerability Disclosure](https://insights.sei.cmu.edu/documents/1945/2017_003_001_503340.pdf) | CERT-CC/Software Engineering Institure (SEI) at Carnegie Mellon University | None - approved for public release and unlimited distribution | Guide | |
| [EUCC Scheme Guidelines on Vulnerability Management and Disclosure](https://certification.enisa.europa.eu/document/download/5f61edd4-0151-4687-8a08-c11c103498f3_en?filename=EUCC_guidelines_vulnerability%20management%20and%20disclosure_v1.1_0.pdf) | European Union Agency for Cybersecurity (ENISA) | CC-BY-ND 4.0 DEED | Guidelines for the EUCC Scheme | Version 1.1 January 2025 - a schema in the European Common Criteria framework |


## Horizontal Type B Standards (due October 30, 2027)

### Making products with digital elements available on the market without known exploitable vulnerabilities

CRA ref: [Annex I, Part I, point (2)(a)][Annex I]\
Standards request ref: 2\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| [FIRST PSIRT Services Framework](https://www.first.org/standards/frameworks/psirts/psirt_services_framework_v1.1) | FIRST | Public Domain | Framework | 2015-present | Guidance on how to create, manage, and operate a Product Security Incident Repsonse Team (PSIRT) |
| [FIRST PSIRT Services Maturity Guidance ](https://www.first.org/standards/frameworks/psirts/psirt_maturity_document) | FIRST | Public Domain | Framework | 2015-present | Guidance on how to demostrate Operational Capabiulity and Maturity for PSIRTs |
| [FIRST CSIRT Services Framework](https://www.first.org/standards/frameworks/csirts/csirt_services_framework_v2.1) | FIRST | Public Domain | Framework | 2015-present | Guidance on how to create, manage, and operate a Computer Security Incident Repsonse Team (CSIRT) |


### Making products with digital elements available on the market with a secure by default configuration

CRA ref: [Annex I, Part I, point (2)(b)][Annex I]\
Standards request ref: 3\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Ensuring that vulnerabilities in products with digital elements can be addressed through security updates

CRA ref: [Annex I, Part I, point (2)(c)][Annex I]\
Standards request ref: 4\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Ensuring protection of products with digital elements from unauthorised access and reporting on possible unauthorised access

CRA ref: [Annex I, Part I, point (2)(d)][Annex I]\
Standards request ref: 5\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Protecting the confidentiality of data stored, transmitted or otherwise processed by a product with digital elements

CRA ref: [Annex I, Part I, point (2)(e)][Annex I]\
Standards request ref: 6\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Protecting the integrity of data, commands, programs by a product with digital elements, and its configuration against any manipulation or modification not authorised by the user, as well as reporting on corruptions

CRA ref: [Annex I, Part I, point (2)(f)][Annex I]\
Standards request ref: 7\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Processing only personal or other data that are adequate, relevant and limited to what is necessary in relation to the intended purpose of the product with digital elements (‘minimisation of data’)

CRA ref: [Annex I, Part I, point (2)(g)][Annex I]\
Standards request ref: 8\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Protecting the availability of essential and basic functions of the product with digital elements

CRA ref: [Annex I, Part I, point (2)(h)][Annex I]\
Standards request ref: 9\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Minimising the negative impact of a product with digital elements or its connected devices on the availability of services provided by other devices or networks

CRA ref: [Annex I, Part I, point (2)(i)][Annex I]\
Standards request ref: 10\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Designing, developing and producing products with digital elements with limitted attack surfaces

CRA ref: [Annex I, Part I, point (2)(j)][Annex I]\
Standards request ref: 11\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Designing, developing and producing products with digital elements that reduce the impact of an incident using appropriate exploitation mitigation mechanisms and techniques

CRA ref: [Annex I, Part I, point (2)(k)][Annex I]\
Standards request ref: 12\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Providing security related information by recording and/or monitoring relevant internal activity of products with digital elements with an opt-out mechanism for the user

CRA ref: [Annex I, Part I, point (2)(l)][Annex I]\
Standards request ref: 13\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Securely and easily removing or transferring all data and settings of a product with digital elements

CRA ref: [Annex I, Part I, point (2)(m)][Annex I]\
Standards request ref: 14\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

## Open Source Steward Cybersecurity policy

CRA ref: [Article 24(1)][Article 24]\
Standards request ref: N/A\
Impact on steward: `obligation`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| [OpenSSF Outbound Vulnerability Disclosure Policy Template](https://github.com/ossf/wg-vulnerability-disclosures/blob/main/docs/Outbound_Vulnerability_Disclosure_Policy_template.md) | OpenSSF | Apache-2.0 | Policy Template | 2024- present | |
| [OpenSSF Security Policy Templates](https://github.com/ossf/oss-vulnerability-guide/tree/main/templates/security_policies) | OpenSSF | Apache-2.0 | Policy Template | 2022- present | |


## Due diligence requirements of manufacturers

CRA ref: [Article 13(5)][Article 13]\
Standards request ref: N/A\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

## Voluntary security attestation programmes

CRA ref: [Article 25][]\
Standards request ref: N/A\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| [FreeBSD SSDF Attestation](https://freebsdfoundation.org/news-and-events/latest-news/freebsd-foundation-announces-ssdf-attestation/) | [FreeBSD Foundation](https://freebsdfoundation.org/) | Confidential | attestation | 2024-11-03 |  |
| [Secure Software Development Framework (SSDF)](https://csrc.nist.gov/projects/ssdf) | [NIST](https://www.nist.gov/) | Public Domain (attribution appreciated) | recommendations | 2022-02-03 |  |

## Other
CRA ref: TBD\
Standards request ref: N/A\
Impact on steward: TBD

_Please add relevant resources below that don't fit well in the other categories. Please explain why they're important in the notes._

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |


[Annex I]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I
[Article 13]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_13
[Article 24]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_24
[Article 25]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_25
