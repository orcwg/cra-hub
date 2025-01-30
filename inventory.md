# Inventory of resources relevant to the horizontal CRA standards, Open Source Steward obligations, and voluntary attestation program

The goal of this document is to collect resources that are relevant to the CRA obligations of _open-source software stewards_ and _manufacturers_ when it comes to the development and usage of open source.

_Please add all relevant resources as a table row under the relevant section or subsection._

## Table of Content

* [Horizontal Type A Standards (due Aug. 2026)](#horizontal-type-a-standards-due-aug-2026)
* [Horizontal Type B Standards (due Sept. 2027)](##horizontal-type-b-standards-due-sept-2027)
* [Open Source Steward Cybersecurity policy](#open-source-steward-cybersecurity-policy)
* [Due diligence requirements of manufacturers](#due-diligence-requirements-of-manufacturers)
* [Voluntary security attestation programmes](#voluntary-security-attestation-programmes)
* [Other](#other)

## General 'meta' guidance

* [CNLL guide to CRA implementation for open soure SMEs](https://code.inno3.eu/ouvert/guide-cra/-/tree/main?ref_type=heads)

## Horizontal Type A Standards (due Aug. 2026)

### Designing, developing and producing products with digital elements in such a way that they ensure an appropriate level of cybersecurity based on the risks

CRA ref: [Annex I, Part I, point (1)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 1\
Impact on steward: `Partial obligation` ("foster development of secure product", [Article. 24(1)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_24))


| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| [OpenStack Secure Development Guidelines](https://security.openstack.org/#secure-development-guidelines) | OpenStack Community | CC-BY-3.0 | informal | 2015-02-18 – present | |
| [OWASP Software Assurance Maturity Model (SAMM)](https://owaspsamm.org) | OWASP | CC-BY-SA-4.0 | Maturity Model | 2009 – present | SAMM is a maturity model that helps organizations implement a Secure Development Lifecycle. |
| [OWASP DevSecOps Maturity Model (DSOMM)](https://dsomm.owasp.org) | OWASP | GPL-3 | Maturity Model | 2017 – present | DSOMM is a maturity model aimed at implementing DevSecOps best practices. |
| [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org) | OWASP | CC BY-SA 4.0 | Informal Guidelines | 2014 – present | OWASP Cheat Sheets are a collection of pragmatic secruity guidelines and best practices for a wide range of technologies. |

### Vulnerability handling for products with digital elements

CRA ref: [Annex I, Part II](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
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
 

## Horizontal Type B Standards (due Sept. 2027)

### Making products with digital elements available on the market without known exploitable vulnerabilities

CRA ref: [Annex I, Part I, point (2)(a)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 2\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Making products with digital elements available on the market with a secure by default configuration

CRA ref: [Annex I, Part I, point (2)(b)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 3\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Ensuring that vulnerabilities in products with digital elements can be addressed through security updates

CRA ref: [Annex I, Part I, point (2)(c)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 4\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Ensuring protection of products with digital elements from unauthorised access and reporting on possible unauthorised access

CRA ref: [Annex I, Part I, point (2)(d)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 5\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Protecting the confidentiality of data stored, transmitted or otherwise processed by a product with digital elements

CRA ref: [Annex I, Part I, point (2)(e)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 6\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Protecting the integrity of data, commands, programs by a product with digital elements, and its configuration against any manipulation or modification not authorised by the user, as well as reporting on corruptions

CRA ref: [Annex I, Part I, point (2)(f)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 7\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Processing only personal or other data that are adequate, relevant and limited to what is necessary in relation to the intended purpose of the product with digital elements (‘minimisation of data’)

CRA ref: [Annex I, Part I, point (2)(g)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 8\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Protecting the availability of essential and basic functions of the product with digital elements

CRA ref: [Annex I, Part I, point (2)(h)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 9\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Minimising the negative impact of a product with digital elements or its connected devices on the availability of services provided by other devices or networks

CRA ref: [Annex I, Part I, point (2)(i)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 10\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Designing, developing and producing products with digital elements with limitted attack surfaces

CRA ref: [Annex I, Part I, point (2)(j)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 11\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Designing, developing and producing products with digital elements that reduce the impact of an incident using appropriate exploitation mitigation mechanisms and techniques

CRA ref: [Annex I, Part I, point (2)(k)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 12\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Providing security related information by recording and/or monitoring relevant internal activity of products with digital elements with an opt-out mechanism for the user

CRA ref: [Annex I, Part I, point (2)(l)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 13\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

### Securely and easily removing or transferring all data and settings of a product with digital elements.

CRA ref: [Annex I, Part I, point (2)(m)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I)\
Standards request ref: 14\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

## Open Source Steward Cybersecurity policy

CRA ref: [Article 24(1)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_24)\
Standards request ref: N/A\
Impact on steward: `obligation`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

## Due diligence requirements of manufacturers

CRA ref: [Article 13(5)](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_24)\
Standards request ref: N/A\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

## Voluntary security attestation programmes

CRA ref: [Article 25](https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_25)\
Standards request ref: N/A\
Impact on steward: `attestations`

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |

## Other
CRA ref: TBD\
Standards request ref: N/A\
Impact on steward: TBD

_Please add relevant resources below that don't fit well in the other categories. Please explain why they're important in the notes._

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
|  |  |  |  |  |  |
