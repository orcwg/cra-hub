# Inventory of resources relevant to development and usage of open source under the Cyber Resilience Act

The goal of this document is to provide a comprehensive list of resources that are relevant to the CRA obligations of open source software stewards and manufacturers when it comes to the development and usage of open source. The underlying purpose is to provide specification and standardization effort with easy access to documented industry and community best practices related to the development and integration of open source software and to the interactions between developers and consumers of open source.

Note: the description of each resource has been generated using a large language model and verified for accuracy.

## Table of Content

* [1. Principles of security resilience][Section 1]
  * [1.1 Risk analysis][Section 1.1]
  * [1.2 Secure design and secure coding principles][Section 1.2]
  * [1.3 Security processes and governance][Section 1.3]
* [2. Generic Security Requirements][Section 2]
  * [2.1 Security requirements and controls][Section 2.1]
  * [2.2 Security Hardening Guidelines][Section 2.2]
  * [2.3 Cryptography][Section 2.3]
* [3. Vulnerability management][Section 3]
  * [3.1 SBOM and Supply chain assurance][Section 3.1]
  * [3.2 Vulnerability handling][Section 3.2]
* [4. Compliance requirements][Section 4.]
  * [4.1 Open Source Steward Cybersecurity policy][Section 4.1]
  * [4.2 Due diligence requirements][Section 4.2]
  * [4.3 Security attestations][Section 4.3]
* [5. Similar legislation][Section 5]
* [6. Other][Section 6]

<!--
## Horizontal Type A Standards (due August 30, 2026)

###



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
-->


## 1. Principles of security resilience

This section contains references which are relevant to the requirements expressed in [Annex I, Part I, point (1)][Annex I] of the CRA:

> Products with digital elements shall be designed, developed and produced in such a way that they ensure an appropriate level of cybersecurity based on the risks.

Standards request ref: [1][Horizontal standards] (Horizontal Type A Standard due August 30, 2026)\
Impact on steward: `Partial obligation` ("foster development of secure product", [Article 24(1)][Article 24])

TODO: CONVERT BELOW TABLE

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| [OWASP DevSecOps Maturity Model (DSOMM)](https://dsomm.owasp.org) | OWASP | GPL-3 | Maturity Model | 2017 – present | DSOMM is a maturity model aimed at implementing DevSecOps best practices. |
| [NIST Secure Software Development Framework (NIST SP 800-218)](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-218.pdf) | National Institute of Standards and Technology (NIST) | No License Required | Guidelines | 2022-02 - present | SSDF is a set of community-derived and regulatory-aligned practices for the creation and usage of software |

* [BSI TR-03183: Cyber Resilience Requirements for Manufacturers and Products](https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/Standards-und-Zertifizierung/Technische-Richtlinien/TR-nach-Thema-sortiert/tr03183/TR-03183_node.html) - This is a German Federal Office for Information Security (BSI) guideline adopted in 2023 to prepare manufacturers for the EU Cyber Resilience Act. It provides detailed requirements and recommendations for product cybersecurity, essentially translating upcoming regulatory expectations into actionable criteria. TR-03183 is divided into parts; Part 1 covers general cyber resilience requirements (e.g. taking a risk-based approach to product security, ensuring secure software development and lifecycle, establishing a vulnerability handling process), and Part 2 focuses specifically on Software Bill of Materials (SBOM) and related transparency measures. The guideline likely also has parts on secure update mechanisms and incident reporting. By following TR-03183, device and software manufacturers can implement baseline security controls (like strong authentication, encryption for data in transit/storage, integrity protections, etc.) and produce artifacts (such as an SBOM) that demonstrate compliance. It effectively serves as an early blueprint for CRA compliance in Germany, giving industry a head-start on meeting those future legal obligations by voluntarily aligning with the technical measures BSI recommends.
  <details>
    <summary>More info</summary>

    * **Title:** BSI TR-03183: Cyber Resilience Requirements for Manufacturers and Products
    * **URL:** https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/Standards-und-Zertifizierung/Technische-Richtlinien/TR-nach-Thema-sortiert/tr03183/TR-03183_node.html
    * **Publisher:** BSI
    * **License:** 
    * **Type:** Formal
    * **Publication date:** 2024
  </details>

* [ETSI 303 645 - Cyber Security for Consumer Internet of Things: Baseline Requirements](https://www.etsi.org/deliver/etsi_en/303600_303699/303645/02.01.01_60/en_303645v020101p.pdf) - ETSI EN 303 645 is a European standard specifying baseline cybersecurity requirements for consumer Internet of Things devices. It enumerates a set of fundamental practices that manufacturers of smart home and wearable devices, for instance, should implement to significantly improve security. Notable provisions include: avoiding universal default passwords (each device must have a unique or user-set credential), providing a means to manage vulnerability disclosure (publish a contact for security issues), keeping software updated (and informing consumers of update duration), securely storing sensitive data, and minimizing exposed attack surfaces. The standard, first released in 2020 (and updated in v2.1.1 to refine requirements), has 13 key provisions in total. While voluntary, EN 303 645 has become highly influential; its guidelines have been adopted or referenced by governments and industry schemes globally (such as in the UK’s and Australia’s IoT codes of practice and Singapore’s CLS levels). In summary, ETSI EN 303 645 serves as a baseline “security hygiene” checklist for IoT products to reduce common vulnerabilities and make consumer devices more resilient against attacks like botnet recruitment or data breaches.
  <details>
    <summary>More info</summary>

    * **Title:** ETSI 303 645 - Cyber Security for Consumer Internet of Things: Baseline Requirements
    * **URL:** https://www.etsi.org/deliver/etsi_en/303600_303699/303645/02.01.01_60/en_303645v020101p.pdf
    * **Publisher:** ETSI
    * **License:** ?
    * **Type:** formal
    * **Publication date:** 2021
  </details>

* [ISO 31000:2018 Risk management — Guidelines](https://www.iso.org/standard/65694.html) - ISO 31000:2018 is an international standard that provides principles and generic guidelines for effective risk management in organizations. Rather than prescribing a specific technique, it outlines a framework and process that organizations can use to identify, assess, and treat risks systematically. Key concepts include establishing the context of risk (understanding the internal and external environment), performing structured risk assessments (identifying risks, analyzing their likelihood and impact, evaluating priorities), and then treating the risks with appropriate controls or mitigation strategies. The standard emphasizes that risk management should be iterative and embedded into organizational processes, decision-making, and culture. By following ISO 31000’s guidelines, organizations of any type can improve their ability to manage uncertainty, minimize losses, and maximize opportunities in a rational, auditable way.
  <details>
    <summary>More info</summary>

    * **Title:**  ISO 31000:2018 Risk management — Guidelines
    * **URL:** https://www.iso.org/standard/65694.html
    * **Publisher:** ISO
    * **License:** ?
    * **Type:** Formal
    * **Publication date:** 2018
  </details>
  

* [NIST 800-37: Risk Management Framework for Information Systems and Organizations: A System Life Cycle Approach for Security and Privacy](https://csrc.nist.gov/pubs/sp/800/37/r2/final) - NIST Special Publication 800-37 Revision 2 is the authoritative guide on applying a Risk Management Framework (RMF) to information systems. The RMF provides a disciplined, structured process that integrates security and privacy into the system development life cycle. The steps of the RMF include: Prepare (organizational and system level preparation for risk management), Categorize (determining the system’s impact level in terms of confidentiality, integrity, availability), Select (choosing an initial set of security and privacy controls from standards like NIST 800-53 based on that categorization and tailoring them as needed), Implement (putting the controls in place), Assess (evaluating how effectively the controls are implemented), Authorize (a senior official formally accepting the residual risk before the system operates), and Monitor (continuously tracking the system’s security posture and control effectiveness over time). Rev. 2 of SP 800-37, published in 2018, updated the process to better support organization-wide risk management, emphasized the importance of privacy, and aligned with the NIST Cybersecurity Framework. It promotes ongoing authorization and continuous monitoring rather than one-time snapshots. Utilizing RMF helps organizations (especially U.S. federal agencies and contractors) ensure that security is not an afterthought but a continuous, lifecycle concern tied to risk decisions.
  <details>
    <summary>More info</summary>

    * **Title:** NIST 800-37: Risk Management Framework for Information Systems and Organizations: A System Life Cycle Approach for Security and Privacy
    * **URL:** https://csrc.nist.gov/pubs/sp/800/37/r2/final
    * **Publisher:** NIST
    * **License:** ?
    * **Type:** informal
    * **Publication date:** 2018
  </details>

* [NIST SP 800-160 Vol. 2 Rev. 1: Developing Cyber-Resilient Systems: A Systems Security Engineering Approach](https://csrc.nist.gov/pubs/sp/800/160/v2/r1/final) - This NIST publication focuses on engineering principles for cyber resilience, complementing traditional cybersecurity (which often emphasizes protection and detection) with strategies to ensure essential functions can withstand and recover from attacks. It adopts a systems security engineering perspective, meaning it embeds resilience into the system design lifecycle. The document introduces a catalog of cyber resiliency techniques and approaches — for example, techniques like redundancy (having backup components), diversity (using different implementations to avoid common-mode failures), segmentation (limiting the blast radius of compromises), deception (confusing or slowing attackers), and graceful degradation (maintaining partial functionality under stress). Rev. 1 updates these concepts and provides use cases and mappings to known frameworks (like mapping resiliency techniques to NIST CSF functions). By applying the guidance in SP 800-160 Vol. 2, system architects and engineers can design systems that continue to operate even while under attack or after compromise, thereby protecting critical missions. The document essentially shifts the focus from just preventing breaches to assuming that incidents will happen and planning how the system will cope and adapt when they do.
  <details>
    <summary>More info</summary>

    * **Title:** NIST SP 800-160 Vol. 2 Rev. 1: Developing Cyber-Resilient Systems: A Systems Security Engineering Approach
    * **URL:** https://csrc.nist.gov/pubs/sp/800/160/v2/r1/final
    * **Publisher:** NIST
    * **License:** ?
    * **Type:** informal
    * **Publication date:** 2021
  </details>

### 1.1 Risk analysis 

* [EN18031 - Common security requirements for radio equipment ](https://www.nen.nl/nen-en-18031-1-2024-en-328074) - EN 18031-1:2024 is a new European harmonized standard developed to support the security provisions of the EU Radio Equipment Directive (RED). As of August 2024, certain radio-connected devices (including many IoT products) must comply with Article 3(3)(d)-(f) of the RED, which mandates network protection, privacy of data, and fraud prevention. EN 18031-1 provides the “common security requirements” that manufacturers can implement to meet these legal obligations. It likely covers a broad set of controls such as requiring authentication for critical functions, ensuring secure data transmission, protecting personal data handled by the equipment, and maintaining software update mechanisms. This standard builds on prior work (like ETSI EN 303 645) but formalizes it under CEN/CENELEC for regulatory conformity. By following EN 18031-1, manufacturers can self-declare or certify that their wireless and IoT products adhere to the necessary cybersecurity baseline, thereby fulfilling the RED requirements and allowing them to be placed on the EU market. Essentially, EN 18031-1 operationalizes the Cyber Resilience Act’s spirit early for radio devices, harmonizing security across all consumer smart products in Europe.
  <details>
    <summary>More info</summary>

    * **Title:** EN18031 - Common security requirements for radio equipment 
    * **URL:** https://www.nen.nl/nen-en-18031-1-2024-en-328074
    * **Publisher:** NEN-EN
    * **License:** ?
    * **Type:** formal
    * **Publication date:** 2024
  </details>

* [OWASP Threat Modeling Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html) - The OWASP Threat Modeling Cheat Sheet is a distilled guide to performing threat modeling, which is the process of systematically identifying and addressing potential threats to an application’s security during the design phase. The cheat sheet outlines the essential steps in threat modeling: defining the security objectives, creating an application diagram or understanding the architecture, identifying threats (often using frameworks like STRIDE: Spoofing, Tampering, Repudiation, Information disclosure, Denial of service, Elevation of privilege), and devising mitigations for those threats. It provides tips and best practices, such as focusing on high-risk assets, involving diverse stakeholders (developers, architects, security engineers), and iterating the threat model as the design evolves. By following this concise guide, developers and teams can ensure they consider security early in the development lifecycle—modeling what could go wrong and building in defenses—rather than reacting to issues late in the game.
  <details>
    <summary>More info</summary>

    * **Title:** OWASP Threat Modeling Cheat Sheet
    * **URL:** https://cheatsheetseries.owasp.org/cheatsheets/Threat_Modeling_Cheat_Sheet.html
    * **Publisher:** OWASP
    * **License:** CC BY-SA 4.0
    * **Type:** informal
    * **Publication date:** ?
  </details>

### 1.2 Secure design and secure coding principles

* [OpenStack Secure development guidelines](https://security.openstack.org/#secure-development-guidelines) - The OpenStack Security Team has created a set of secure development guidelines and best practices to help developers avoid common mistakes that could introduce vulnerabilities in the OpenStack platform. These guidelines cover various areas of secure coding (e.g. proper file permissions, input validation, avoiding insecure libraries, using encryption correctly) and serve as a baseline for developers to follow so that OpenStack components are built with security in mind. By adhering to these recommendations, contributors to OpenStack can systematically reduce security weaknesses and improve the overall resilience of the cloud software.
  <details>
    <summary>More info</summary>

    * **Title:** OpenStack Secure development guidelines
    * **URL:** https://security.openstack.org/#secure-development-guidelines
    * **Publisher:** OpenStack Community
    * **License:** CC-BY-3.0
    * **Type:** informal
    * **Publication date:** 2015-02-18 – present
  </details>
  
* [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/) - The OWASP Cheat Sheet Series is a collection of concise, high-value guides on a wide range of application security topics. Each cheat sheet focuses on a specific area (for example, authentication, injection prevention, error handling, etc.) and distills essential best practices and recommendations in an easy-to-reference format. Created and maintained by security experts in the OWASP community, the cheat sheets provide developers and defenders with clear guidelines to implement security controls correctly. By following the Cheat Sheet Series, practitioners can quickly learn the do’s and don’ts of application security for common scenarios, thereby improving the security of software without needing to wade through extensive documentation.
  <details>
    <summary>More info</summary>

    * **Title:** OWASP Cheat Sheet Series
    * **URL:** https://cheatsheetseries.owasp.org/
    * **Publisher:** OWASP
    * **License:** CC BY-SA 4.0
    * **Type:** informal
    * **Publication date:** 2014 – present
  </details>

### 1.3 Security processes and governance

* [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework) - The NIST CSF is a high-level framework that helps organizations manage and reduce cybersecurity risk. It is composed of five Core Functions: Identify (know your assets, systems, data, and risks), Protect (implement safeguards like access controls, training, maintenance), Detect (deploy activities to promptly detect anomalies and incidents), Respond (have plans and actions for containing and minimizing incidents), and Recover (restore any capabilities or services impaired by incidents and incorporate lessons learned). Under each function are Categories and Subcategories that outline specific outcomes (for example, under Protect -> Access Control, an outcome is “identities and credentials are managed for authorized devices and users”). The CSF also includes Implementation Tiers to gauge the maturity of risk management practices and a Profile concept to tailor the framework to the organization’s goals and sector. Initially developed for critical infrastructure, the CSF has been widely adopted across industries globally because of its flexibility and clear structure. It’s often used as a starting point for developing a cybersecurity program or as a communication tool between technical teams and management, since it distills complex security practices into a straightforward, business-aligned format. (Note: A CSF 2.0 update is underway to incorporate more guidance on governance and supply chain risk.)
  <details>
    <summary>More info</summary>

    * **Title:** NIST Cybersecurity Framework
    * **URL:** https://www.nist.gov/cyberframework
    * **Publisher:** NIST
    * **License:** ?
    * **Type:** informal
    * **Publication date:** Ongoing
  </details>

* [OWASP Software Assurance Maturity Model (SAMM)](https://owaspsamm.org/) - OWASP SAMM is an open framework that organizations use to evaluate and improve their software security practices. It defines 15 security practices grouped into 5 business functions (such as Governance, Design, Implementation, Verification, and Operations), each with maturity levels and activities. By assessing their maturity against SAMM’s criteria, organizations can identify gaps in how they design, develop, and deploy software, and then follow SAMM’s guidance to incrementally implement more advanced security practices. The model is technology-agnostic and is updated by the OWASP community to reflect current best practices, making it a versatile roadmap for building a robust software security assurance program.
  <details>
    <summary>More info</summary>

    * **Title:** OWASP Software Assurance Maturity Model (SAMM)
    * **URL:** https://owaspsamm.org/
    * **Publisher:** OWASP
    * **License:** CC-BY-SA 4.0
    * **Type:** informal
    * **Publication date:** 2009 – present
  </details>

## 2. Generic Security Requirements

### 2.1 Security requirements and controls

### 2.2 Security Hardening Guidelines

### 2.3 Cryptography
 
## 3. Vulnerability management

* [CISA Software Acquisition Guide](https://cisa.gov/sag) - _See full description in [Section 4.2 Due diligence requirements][Section 4.2]._

### 3.1 SBOM and Supply chain assurance

### 3.2 Vulnerability handling

## 4. Compliance requirements

* [Cyber Resilience Act Compliance Guide for Open Source](https://code.inno3.eu/ouvert/guide-cra/-/raw/main/CNLL_inno3_Guide-CRA_VE_1.0.pdf?ref_type=heads&inline=false) - This guide, put together by European open source advocacy groups, interprets the EU Cyber Resilience Act (CRA) through the lens of open source software development. The CRA will impose certain security and compliance requirements on “products with digital elements.” Many open source maintainers are concerned about how to meet these obligations. The guide likely breaks down the CRA’s key requirements – such as providing security support and updates for a product, having a vulnerability disclosure process, ensuring the software is developed following secure practices, and including technical documentation – and offers suggestions for open source projects to address them. It might recommend things like adopting an open source security best practices badge (to show development follows guidelines), publishing an SBOM for releases, clearly stating how users will be alerted to issues or updates, and possibly working with downstream distributors who can help fulfill CRA duties. It also may clarify which open source scenarios are out of scope of the CRA (for example, maybe software provided without commercial intent). In short, this compliance guide serves as a bridge to help the open source community understand and prepare for the new regulatory landscape under the CRA, aiming to ensure that open source can remain sustainable and trusted under these rules.
  <details>
    <summary>More info</summary>

    * **Title:** Cyber Resilience Act Compliance Guide for Open Source
    * **URL:** https://code.inno3.eu/ouvert/guide-cra/-/raw/main/CNLL_inno3_Guide-CRA_VE_1.0.pdf?ref_type=heads&inline=false
    * **Publisher:** inno³ and CNLL,
    * **License:** CC-by-SA 4.0
    * **Type:** 
    * **Publication date:** 2024
  </details>

### 4.1 Open Source Steward Cybersecurity policy

CRA ref: [Article 24(1)][Article 24]\
Standards request ref: N/A\
Impact on steward: `obligation`

TODO: CONVERT BELOW TABLE

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| [OpenSSF Outbound Vulnerability Disclosure Policy Template](https://github.com/ossf/wg-vulnerability-disclosures/blob/main/docs/Outbound_Vulnerability_Disclosure_Policy_template.md) | OpenSSF | Apache-2.0 | Policy Template | 2024- present | |
| [OpenSSF Security Policy Templates](https://github.com/ossf/oss-vulnerability-guide/tree/main/templates/security_policies) | OpenSSF | Apache-2.0 | Policy Template | 2022- present | |


### 4.2 Due diligence requirements

CRA ref: [Article 13(5)][Article 13]\
Standards request ref: N/A\
Impact on steward: `attestations`

* [CISA Software Acquisition Guide](https://cisa.gov/sag) - The U.S. CISA Software Acquisition Guide provides practical guidance to government agencies (and large enterprises) on how to incorporate security considerations into the procurement of software. It outlines how buyers should define security requirements in RFPs/contracts – such as requiring vendors to follow secure development standards (like the NIST SSDF), provide artifacts like SBOMs and vulnerability disclosure policies, and agree to notify and patch if vulnerabilities are found. It also advises on evaluating supplier risk (e.g. checking if the vendor has had frequent security issues historically or if they have certified processes like ISO 27001). The guide suggests structuring the vendor selection process to include security questionnaires or assessments and to prefer vendors who can demonstrate secure-by-design approaches (perhaps via certifications or past performance). Additionally, it covers how to handle acquired software: establishing processes for incoming SBOM analysis, periodic re-scans for vulnerabilities in the product, and ensuring maintenance contracts cover security updates. By following this guide, procurement officers and risk managers can make more informed decisions, selecting products that not only meet functionality needs but also contribute positively to the organization’s security posture, thereby using market forces to encourage vendors to deliver safer software.
  <details>
    <summary>More info</summary>

    * **Title:** US CISA Software Acquisition Guide
    * **URL:** https://cisa.gov/sag
    * **Publisher:** CISA
    * **License:** 
    * **Type:** 
    * **Publication date:** 2024
  </details>

* [Good Practices in Supply Chain Cybersecurity](https://www.enisa.europa.eu/sites/default/files/publications/Good%20Practices%20for%20Supply%20Chain%20Cybersecurity.pdf) - This report by the European Union Agency for Cybersecurity (ENISA) surveys the threat landscape of ICT supply chains and offers recommendations to secure them. It identifies common attack scenarios and weaknesses in digital supply chains (such as compromise of third-party software dependencies, insecure equipment from suppliers, or poor internal supplier security processes). The document then presents a set of good practices for different stakeholders – including manufacturers, service providers, and customers – to mitigate these risks. These practices range from performing due diligence and security audits on suppliers, incorporating security requirements into procurement contracts, ensuring suppliers have vulnerability management and incident response procedures, to establishing multi-tier trust (so that suppliers enforce similar standards on their subcontractors). By following these practices, organizations can strengthen the weakest links in their supply chain and reduce the risk of cascading security incidents originating from outside partners or components.
  <details>
    <summary>More info</summary>

    * **Title:** Good Practices in Supply Chain Cybersecurity
    * **URL:** https://www.enisa.europa.eu/sites/default/files/publications/Good%20Practices%20for%20Supply%20Chain%20Cybersecurity.pdf
    * **Publisher:** ENISA
    * **License:** CC-BY-4.0
    * **Type:** 
    * **Publication date:** 2023 – present
  </details>

### 4.3 Security attestations

CRA ref: [Article 25][]\
Standards request ref: N/A\
Impact on steward: `attestations`

TODO: CONVERT BELOW TABLE

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| [FreeBSD SSDF Attestation](https://freebsdfoundation.org/news-and-events/latest-news/freebsd-foundation-announces-ssdf-attestation/) | [FreeBSD Foundation](https://freebsdfoundation.org/) | Confidential | attestation | 2024-11-03 |  |
| [Secure Software Development Framework (SSDF)](https://csrc.nist.gov/projects/ssdf) | [NIST](https://www.nist.gov/) | Public Domain (attribution appreciated) | recommendations | 2022-02-03 |  |

* [Best Practices Badge](https://www.bestpractices.dev/en) - The OpenSSF Best Practices Badge Program is a voluntary self-certification initiative that allows open-source software projects to demonstrate their adherence to a broad range of security and quality best practices. Projects complete a web-based questionnaire covering topics like version control, vulnerability disclosure, testing, code review, and build process hygiene. If they meet the criteria, they earn a badge that can be displayed to indicate the project follows industry-recommended practices for open source development. The program (originating from the Core Infrastructure Initiative and now under the Open Source Security Foundation) aims to improve software health and transparency; consumers of open source can use the badge as one indicator that a project is more likely to produce secure, reliable software.
  <details>
    <summary>More info</summary>

    * **Title:** Best Practices Badge
    * **URL:** https://www.bestpractices.dev/en
    * **Publisher:** OpenSSF
    * **License:** MIT/CDLA-Permissive
    * **Type:** 
    * **Publication date:** from 2021 under the current name
  </details>
  
* [Authoritative Guide to Attestations](https://cyclonedx.org/guides/OWASP_CycloneDX-Authoritative-Guide-to-Attestations-en.pdf) - This guide provides organizations with a framework for digitally transforming their audit and attestation workflows using standardized, machine-readable attestations. An attestation in this context is a cryptographically signed statement about some aspect of a software product or process (for example, an attestation that a product was built in a secure environment or complies with certain standards). The guide explains how to create and use such attestations, leveraging the CycloneDX format, to document compliance or security assurances in an automated way. By following the guide, organizations can move away from purely manual audit statements and instead generate verifiable digital evidence of their security practices, making it easier to trust and verify software in supply chains or regulatory contexts.
  <details>
    <summary>More info</summary>

    * **Title:** Authoritative Guide to Attestations
    * **URL:** https://cyclonedx.org/guides/OWASP_CycloneDX-Authoritative-Guide-to-Attestations-en.pdf
    * **Publisher:** OWASP
    * **License:** CC-BY-SA 4.0
    * **Type:** informal
    * **Publication date:** 2024 – present
  </details>

## 5. Similar legislation

## 6. Other

[Section 1]:   #1-principles-of-security-resilience
[Section 1.1]: #11-risk-analysis
[Section 1.2]: #12-secure-design-and-secure-coding-principles
[Section 1.3]: #13-security-processes-and-governance
[Section 2]:   #2-generic-security-requirements
[Section 2.1]: #21-security-requirements-and-controls
[Section 2.2]: #22-security-hardening-guidelines
[Section 2.3]: #23-cryptography
[Section 3]:   #3-vulnerability-management
[Section 3.1]: #31-sbom--supply-chain-assurance
[Section 3.2]: #32-vulnerability-handling
[Section 4.]:  #4-compliance-requirements
[Section 4.1]: #41-open-source-steward-cybersecurity-policy
[Section 4.2]: #42-due-diligence-requirements
[Section 4.3]: #43-security-attestations
[Section 5]:   #5-similar-legislation
[Section 6]:   #6-other

[Annex I]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#anx_I
[Article 13]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_13
[Article 24]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_24
[Article 25]: https://eur-lex.europa.eu/legal-content/EN/TXT/HTML/?uri=OJ:L_202402847#art_25

[Horizontal standards]: https://github.com/orcwg/cra-hub/blob/main/standards.md#milestone-1---horizontal-standards-due-august-30-2026
[Vertical standards]: https://github.com/orcwg/cra-hub/blob/main/standards.md#milestone-2---vertical-standards-due-october-30-2026
[Type B standards]: https://github.com/orcwg/cra-hub/blob/main/standards.md#milestone-3---horizontal-standards-due-october-30-2027