# Inventory of resources relevant to development and usage of open source under the Cyber Resilience Act

The goal of this document is to provide a comprehensive list of resources that are relevant to the CRA obligations of open source software stewards and manufacturers when it comes to the development and usage of open source. The underlying purpose is to provide specification and standardization effort with easy access to documented industry and community best practices related to the development and integration of open source software and to the interactions between developers and consumers of open source.

Note: the description of each resource has been generated using a large language model and verified for accuracy. See [Annex I](#annex-i) below for the prompt used.

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




## Horizontal Type B Standards (due October 30, 2027)

### Making products with digital elements available on the market without known exploitable vulnerabilities

CRA ref: [Annex I, Part I, point (2)(a)][Annex I]\
Standards request ref: 2\
Impact on steward: `attestations`

### Making products with digital elements available on the market with a secure by default configuration

CRA ref: [Annex I, Part I, point (2)(b)][Annex I]\
Standards request ref: 3\
Impact on steward: `attestations`



### Ensuring that vulnerabilities in products with digital elements can be addressed through security updates

CRA ref: [Annex I, Part I, point (2)(c)][Annex I]\
Standards request ref: 4\
Impact on steward: `attestations`



### Ensuring protection of products with digital elements from unauthorised access and reporting on possible unauthorised access

CRA ref: [Annex I, Part I, point (2)(d)][Annex I]\
Standards request ref: 5\
Impact on steward: `attestations`



### Protecting the confidentiality of data stored, transmitted or otherwise processed by a product with digital elements

CRA ref: [Annex I, Part I, point (2)(e)][Annex I]\
Standards request ref: 6\
Impact on steward: `attestations`



### Protecting the integrity of data, commands, programs by a product with digital elements, and its configuration against any manipulation or modification not authorised by the user, as well as reporting on corruptions

CRA ref: [Annex I, Part I, point (2)(f)][Annex I]\
Standards request ref: 7\
Impact on steward: `attestations`



### Processing only personal or other data that are adequate, relevant and limited to what is necessary in relation to the intended purpose of the product with digital elements (‘minimisation of data’)

CRA ref: [Annex I, Part I, point (2)(g)][Annex I]\
Standards request ref: 8\
Impact on steward: `attestations`



### Protecting the availability of essential and basic functions of the product with digital elements

CRA ref: [Annex I, Part I, point (2)(h)][Annex I]\
Standards request ref: 9\
Impact on steward: `attestations`



### Minimising the negative impact of a product with digital elements or its connected devices on the availability of services provided by other devices or networks

CRA ref: [Annex I, Part I, point (2)(i)][Annex I]\
Standards request ref: 10\
Impact on steward: `attestations`



### Designing, developing and producing products with digital elements with limitted attack surfaces

CRA ref: [Annex I, Part I, point (2)(j)][Annex I]\
Standards request ref: 11\
Impact on steward: `attestations`



### Designing, developing and producing products with digital elements that reduce the impact of an incident using appropriate exploitation mitigation mechanisms and techniques

CRA ref: [Annex I, Part I, point (2)(k)][Annex I]\
Standards request ref: 12\
Impact on steward: `attestations`



### Providing security related information by recording and/or monitoring relevant internal activity of products with digital elements with an opt-out mechanism for the user

CRA ref: [Annex I, Part I, point (2)(l)][Annex I]\
Standards request ref: 13\
Impact on steward: `attestations`



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

TODO: DOCUMENT HOW THIS CATEGORY IS BROKEN DOWN AND WHY

| Name & URL | Publisher | License | Type | Date | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| [FIRST PSIRT Services Framework](https://www.first.org/standards/frameworks/psirts/psirt_services_framework_v1.1) | FIRST | Public Domain | Framework | 2015-present | Guidance on how to create, manage, and operate a Product Security Incident Repsonse Team (PSIRT) |
| [FIRST PSIRT Services Maturity Guidance ](https://www.first.org/standards/frameworks/psirts/psirt_maturity_document) | FIRST | Public Domain | Framework | 2015-present | Guidance on how to demostrate Operational Capabiulity and Maturity for PSIRTs |
| [FIRST CSIRT Services Framework](https://www.first.org/standards/frameworks/csirts/csirt_services_framework_v2.1) | FIRST | Public Domain | Framework | 2015-present | Guidance on how to create, manage, and operate a Computer Security Incident Repsonse Team (CSIRT) |

### 2.1 Security requirements and controls

* [Hardware Secure Boot](https://www.opencompute.org/documents/secure-boot-2-pdf) - This guide from the Open Compute Project (OCP) provides design requirements and recommendations for implementing secure boot in hardware systems (like servers or network devices). Secure boot is a mechanism where the system’s boot firmware (BIOS/UEFI or similar) will only execute code that is cryptographically signed by a trusted authority. The OCP guide likely details how to establish a root of trust in hardware (such as using a TPM or dedicated secure element to store cryptographic keys), how to sign bootloaders and OS kernels, and how the verification process should work at each stage of the boot chain. It may also discuss managing keys (for example, allowing owners to enroll their own keys or update keys securely) and handling firmware updates in a secure manner (ensuring updates are signed and verified). By adhering to this guide, manufacturers can ensure their devices are protected against low-level malware: even if an attacker has physical access or can alter the boot device, the system will refuse to run untrusted boot code, thus preventing persistent malware like rootkits from taking hold. In summary, the OCP Secure Boot Guide is a blueprint for building devices that only run authentic, untampered software from power-on through full system startup.
  <details>
    <summary>More info</summary>

    * **Title:** Hardware Secure Boot
    * **URL:** https://www.opencompute.org/documents/secure-boot-2-pdf
    * **Publisher:** OpenCompute
    * **License:** 
    * **Type:** informal
    * **Publication date:** 
  </details>

* [NIST SP 800-53 Rev. 5: Security and Privacy Controls for Information Systems and Organizations](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final) - NIST SP 800-53 is a comprehensive catalog of controls (safeguards and countermeasures) that organizations can apply to protect information systems and personal data. Revision 5, released in 2020, expanded the catalog to integrate privacy fully alongside security and made the language more outcome-based (less federal-centric), so it’s usable by a wider audience (government, industry, international). The catalog is organized into families like Access Control, Incident Response, Cryptography, Personnel Security, etc., each containing specific controls. For example, in Access Control, one control is implementing role-based access with the principle of least privilege. Rev. 5 introduced new control families for areas like Supply Chain Risk Management, refined controls for advanced technologies (IoT, mobile), and removed the concept of “low/medium/high baselines” from the document itself (that moved to separate guidance) to focus on the controls. An organization using SP 800-53 will select a subset of these controls based on its risk assessment (often guided by frameworks like SP 800-37 RMF) and then implement and document them. SP 800-53 is widely used not only by U.S. federal agencies (it’s the backbone of FedRAMP, DoD, etc. requirements) but also by others as a rich reference of security best practices to draw from when securing systems.
  <details>
    <summary>More info</summary>

    * **Title:** NIST SP 800-53 Rev. 5: Security and Privacy Controls for Information Systems and Organizations
    * **URL:** https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final
    * **Publisher:** NIST
    * **License:** ?
    * **Type:** informal
    * **Publication date:** 2020
  </details>

* [OWASP Application Security Verification Standard](https://owasp.org/www-project-application-security-verification-standard/) - The OWASP ASVS is a framework that provides a checklist of application security requirements and controls in a structured manner, serving as a basis for testing web application security. It defines three levels of verification depth: Level 1 (basic, for all applications) through Level 3 (advanced, for the most critical applications). Each level comprises requirements across categories such as Authentication, Access Control, Data Protection, Error Handling, and others. For example, at Level 1, there might be a requirement that the application has no default passwords and uses HTTPS; at higher levels, requirements become more stringent, like implementing strong multi-factor authentication, or using cryptographic modules with specific certifications. Developers and architects can use ASVS during development to ensure they build in these controls, and security testers can use it as a guide for what to verify (it’s often used to structure penetration testing or security code review efforts). By using ASVS, organizations get a common language for what it means for an application to be “secure” at a given level, and they can assert compliance to that level. Ultimately, ASVS helps raise the security baseline by providing clear, measurable security criteria for applications.
  <details>
    <summary>More info</summary>

    * **Title:** OWASP Application Security Verification Standard
    * **URL:** https://owasp.org/www-project-application-security-verification-standard/
    * **Publisher:** OWASP
    * **License:** CC BY-SA 3.0
    * **Type:** 
    * **Publication date:** 
  </details>

### 2.2 Security Hardening Guidelines

### 2.3 Cryptography
 
## 3. Vulnerability management

TODO: CONVERT BELOW TABLE


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

## 5. Similar legislation

### Australia

* [Australia Code of Practice - Securing the Internet of Things for Consumers]() - Australia released a voluntary Code of Practice for consumer IoT security in 2020 (developed by the Department of Home Affairs). This code closely mirrors the UK’s 13 IoT security principles and ETSI’s guidelines. It includes practices such as: don’t use default passwords (and preferably implement unique passwords per device), implement a vulnerability disclosure policy, keep software updated and securely updateable, securely store credentials, minimize data collection, and ensure devices can be securely deleted or reset by users. The Australian Code of Practice serves as guidance for industry; while not legally binding, it was endorsed by the government as the expected norm. Companies are encouraged to adopt it and even use it as a competitive advantage (demonstrating compliance could be marketed to consumers). The code also set the stage for potential future regulation if voluntary uptake is insufficient. By articulating clear best practices, Australia’s government aimed to elevate IoT security and protect Australian consumers from common IoT threats like unauthorized access or data breaches via their smart devices. The principles from this code of practice have since influenced discussions on IoT security regulation and labeling in Australia (such as the work towards an IoT security “star rating” similar to other countries).
  <details>
    <summary>More info</summary>

    * **Title:** Australia Code of Practice - Securing the Internet of Things for Consumers
    * **URL:** 
    * **Publisher:** 
    * **License:** 
    * **Type:** 
    * **Publication date:** 
  </details>
  
### Finland

  * [Finland’s national consumer IoT certification scheme]() -  Finland was a pioneer in Europe for consumer IoT security certification, launching its cybersecurity label program in 2019. In this scheme run by Traficom (the Finnish Transport and Communications Agency), manufacturers can apply to have their smart products evaluated against a set of security criteria. Certified products receive a “Cybersecurity Label” (Tietoturvamerkki in Finnish) that they can display to inform consumers that the device meets Finland’s security requirements. The criteria include things like no default passwords, secure communications, and a commitment by the vendor to update the product’s software to fix vulnerabilities. The Finnish label is voluntary but has seen adoption in products like smart watches, home hubs, and IoT appliances. The program’s goal is to raise consumer awareness and reward companies that invest in security. Finland’s label has gained international recognition – it has mutual recognition with Singapore’s CLS (whereby a product meeting the Finnish label is accepted as Level 3 in Singapore’s scheme). This national certification helps build trust in IoT products and influenced the development of similar labeling efforts across the EU.
    <details>
      <summary>More info</summary>

      * **Title:** Finland’s national consumer IoT certification scheme
      * **URL:** 
      * **Publisher:** 
      * **License:** 
      * **Type:** 
      * **Publication date:** 
    </details>
    
### Germany
  
  * [Germany BSI IoT label](https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/IT-Sicherheitskennzeichen/it-sicherheitskennzeichen_node.html) - The German Federal Office for Information Security (BSI) introduced an “IT-Sicherheitskennzeichen” (IT Security Label) in 2022 for consumer IT products. This is a voluntary label that manufacturers can obtain to signal that their product meets basic cybersecurity requirements and that the manufacturer is transparent about its security features. Rather than extensive lab testing, the BSI label currently works as a self-declaration: the manufacturer commits to certain practices (for example, providing software updates for a minimum period, and having no universal default passwords) and BSI publishes a webpage for each labeled product detailing its security properties and update policy. The label itself is often a QR code that consumers can scan to read those details on BSI’s website. This approach educates consumers on what the device does for security and what they as users should do (like applying updates). Products like routers, smart TVs, and cameras have started getting the label. The label program also ties into international efforts: Germany and Singapore have a mutual recognition arrangement (devices with Germany’s label count as at least CLS Level 2 in Singapore and vice versa). Overall, the BSI IT Security Label aims to increase IoT product security through transparency and by pushing manufacturers to adhere to baseline good practices in order to earn the official recognition.
    <details>
      <summary>More info</summary>

      * **Title:** Germany BSI IoT label
      * **URL:** https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/IT-Sicherheitskennzeichen/it-sicherheitskennzeichen_node.html
      * **Publisher:** 
      * **License:** 
      * **Type:** 
      * **Publication date:** 
    </details>
  
### India

* [CSCRF for SEBI REs](https://www.sebi.gov.in/legal/circulars/aug-2024/cybersecurity-and-cyber-resilience-framework-cscrf-for-sebi-regulated-entities-res-_85964.html) - Introduced by the Securities and Exchange Board of India in August 2024, the CSCRF is a comprehensive framework of cybersecurity guidelines for India’s capital market entities (stock exchanges, depositories, brokers, asset managers, etc.). It mandates that these regulated entities implement uniform baseline measures to anticipate cyber threats, protect systems, detect incidents, respond to attacks, and recover operations – aligning with broader cyber resilience goals. The CSCRF sets out objectives like addressing evolving threats, aligning with international standards, enforcing regular cybersecurity audits, and standardizing incident reporting. It introduces structured requirements by combining Cyber Resilience Goals (Anticipate, Withstand, Recover, Evolve) with Cybersecurity Functions (such as Governance, Identify, Protect, Detect, Respond). Entities are categorized by size/impact and must implement controls appropriate to their category. Overall, this framework elevates the cybersecurity posture of India’s financial sector by requiring consistent practices and accountability across all regulated organizations.
  <details>
    <summary>More info</summary>

    * **Title:** CSCRF for SEBI REs
    * **URL:** https://www.sebi.gov.in/legal/circulars/aug-2024/cybersecurity-and-cyber-resilience-framework-cscrf-for-sebi-regulated-entities-res-_85964.html
    * **Publisher:** SEBI
    * **License:** 
    * **Type:** Formal
    * **Publication date:** 45524
  </details>
  
* [TEC Code of Practice for Securing Consumer IoT]() - India’s Telecommunication Engineering Centre (TEC), under the Department of Telecom, released a “Code of Practice” in January 2022 as a guideline for consumer IoT security. This code of practice is largely aligned with global benchmarks like ETSI EN 303 645 and the UK’s 13 principles for IoT security. It provides a list of best practices that manufacturers should implement: some examples include using unique per-device passwords, implementing a vulnerability disclosure mechanism, securing personal data, ensuring communications are encrypted, and providing software updates to devices. While not a regulation, this document serves as an official reference for what the Indian government expects in terms of IoT device security. It’s intended for device manufacturers, IoT service providers, and app developers to consult and adopt these measures in their products and services. By following the TEC’s code, IoT companies can significantly raise the security level of their products in India, and it prepares them for any future mandatory requirements. The issuance of this guideline reflects India’s recognition of the growing risks posed by the proliferation of IoT devices and the need to protect consumers and critical networks from those risks.
  <details>
    <summary>More info</summary>

    * **Title:** India TEC Code of Practice for Securing Consumer IoT
    * **URL:** 
    * **Publisher:** 
    * **License:** 
    * **Type:** 
    * **Publication date:** 
  </details>
  
### United Kingdom

* [U.K.’s Product Security and Telecommunications Infrastructure Bill]() - The UK PSTI Act 2022 is a landmark law that establishes cybersecurity requirements for consumer connectable products (the IoT devices). Building on prior voluntary guidelines, it makes certain practices legally mandatory for manufacturers, importers, and distributors in the UK. The Act’s first set of requirements (which will be enforced via secondary regulations) include: banning universal default passwords in devices, requiring a public point of contact for vulnerability reporting, and mandating transparency about the minimum time period during which the device will receive security updates. Manufacturers must provide a compliance statement for their products covering these aspects. The law gives regulators power to fine companies that don’t comply. Essentially, PSTI turns basic IoT security principles into law – for example, if a toy or appliance ships with a default password like “admin” that is not unique, that will be illegal to sell in the UK. The Act also gives the government flexibility to expand requirements over time (it can add further provisions like mandates around data encryption or firewalls if needed). By legislating these measures, the UK aims to remove the most egregious vulnerabilities from consumer devices and drive manufacturers globally to improve the security of the products that end up in British households.
  <details>
    <summary>More info</summary>

    * **Title:** U.K.’s Product Security and Telecommunications Infrastructure Bill
    * **URL:** 
    * **Publisher:** 
    * **License:** 
    * **Type:** 
    * **Publication date:** 
  </details>

### United States of America

* [CISA Secure by Design Pledge](https://www.cisa.gov/sites/default/files/2024-05/CISA%20Secure%20by%20Design%20Pledge_508c.pdf) - The Secure by Design pledge is an initiative by the U.S. Cybersecurity and Infrastructure Security Agency calling on technology companies to fundamentally shift their development philosophy to prioritize security from the start. The pledge outlines core principles such as developing software with a proactive adversary mindset (anticipating how software could be misused or attacked), ensuring default configurations are secure out-of-the-box (so customers don’t have to harden products themselves), practicing transparency in vulnerability handling (including publishing SBOMs and disclosing vulnerabilities), and enabling continuous security testing and feedback during development. Companies that take the pledge publicly commit to these values, signaling that they will invest in practices like threat modeling, secure coding training, rigorous testing, and building security features (like authentication and encryption) as integral parts of their products. The broader goal is cultural: to move the industry away from treating security as an afterthought or add-on, and instead have security as a foundational aspect of product design, thereby reducing the prevalence of easily exploitable weaknesses in widely used technology.
  <details>
    <summary>More info</summary>

    * **Title:** CISA Secure by Design Pledge
    * **URL:** https://www.cisa.gov/sites/default/files/2024-05/CISA%20Secure%20by%20Design%20Pledge_508c.pdf
    * **Publisher:** CISA
    * **License:** 
    * **Type:** 
    * **Publication date:** 2024
  </details>

* [Cybersecurity Labelling Scheme for IoT - CLS(IoT)](https://www.csa.gov.sg/our-programmes/certification-and-labelling-schemes/cybersecurity-labelling-scheme/about/) - Singapore’s Cybersecurity Labelling Scheme is a four-tier rating program launched in 2020 by the Cyber Security Agency (CSA) to improve the security of consumer smart devices. Under CLS, IoT products (like home routers, smart cameras, etc.) are evaluated and given a security grade of Level 1 (basic) to Level 4 (most robust), indicated by the number of stars on the label. Each level corresponds to a set of cybersecurity provisions: for example, Level 1 requires adherence to baseline security requirements (largely based on ETSI EN 303 645), higher levels add requirements like using a vetted standard (Level 2), conducting structured lifecycle security measures and binary analysis (Level 3), and perhaps formal certification or penetration testing (Level 4). The label helps consumers easily identify products with better cybersecurity and incentivizes manufacturers to incorporate stronger security into design to achieve higher ratings. Singapore’s CLS is one of the first schemes of its kind in Asia and includes mutual recognition arrangements (e.g., a device meeting Finland’s cybersecurity label is recognized at CLS Level 3, and vice versa), promoting international coherence in IoT security standards.
  <details>
    <summary>More info</summary>

    * **Title:** Cybersecurity Labelling Scheme for IoT - CLS(IoT)
    * **URL:** https://www.csa.gov.sg/our-programmes/certification-and-labelling-schemes/cybersecurity-labelling-scheme/about/
    * **Publisher:** CSA
    * **License:** 
    * **Type:** Formal
    * **Publication date:** 
  </details>

* [CyberTrust Mark](https://www.fcc.gov/CyberTrustMark) - The Cyber Trust Mark is a forthcoming labeling scheme introduced by the U.S. Federal Communications Commission (FCC) to signify consumer IoT products that meet certain cybersecurity benchmarks. Under this program, makers of smart devices (like smart thermostats, fitness trackers, connected appliances, etc.) can voluntarily undergo an evaluation of their product’s security features. The baseline criteria likely include things like: unique default passwords or user setup of credentials, a commitment to provide security updates for a minimum period, having a vulnerability reporting mechanism, and perhaps compliance with standards such as ETSI EN 303 645. Devices that pass the evaluation will be allowed to display the “Cyber Trust Mark” logo (possibly a shield icon or similar) on their packaging. This functions similarly to an EnergyStar label but for cybersecurity. The idea is to help consumers easily identify products that are deemed more secure, thereby encouraging manufacturers to improve security to earn the mark. Over time, widespread adoption of the Cyber Trust Mark aims to raise the minimum security level of IoT devices available in the U.S. market by combining consumer choice with a recognizable seal of approval for security.
  <details>
    <summary>More info</summary>

    * **Title:** CyberTrust Mark
    * **URL:** https://www.fcc.gov/CyberTrustMark
    * **Publisher:** US FCC
    * **License:** 
    * **Type:** formal
    * **Publication date:** 2023
  </details>

* [Executive Order 14144 - Strengthening and Promoting Innovation in the Nation's Cybersecurity](https://www.federalregister.gov/documents/2025/01/17/2025-01470/strengthening-and-promoting-innovation-in-the-nations-cybersecurity#p-10) - A key aspect of Executive Order 14144 is its directive to federal procurement authorities to define and enforce criteria for “secure and trustworthy” products. The Executive Order mandates that federal agencies, when buying software or connected devices, must ensure those products meet rigorous cybersecurity standards – effectively using government contracts as a driver for better security. It tasks NIST and other agencies with establishing what technical evidence or certifications a vendor must provide to be considered trustworthy. This could include providing an SBOM for supplied software, proving that the software was developed under secure processes (via self-attestation or third-party audit), demonstrating compliance with specific standards (like FIPS-validated cryptography, or adherence to zero-trust principles if relevant), and ensuring mechanisms for swift vulnerability remediation. The Federal Acquisition Regulation (FAR) will be updated accordingly, making these requirements legally binding in contracts. In practical terms, this means a software company wanting to sell to the U.S. government will need to implement robust security in their product and supply chain or risk being excluded. The intent is both to protect government systems from supply chain attacks and to influence the broader market: when large vendors improve security to sell to the government, those improvements often propagate to all customers.
  <details>
    <summary>More info</summary>

    * **Title:** EO 14144
    * **URL:** https://www.federalregister.gov/documents/2025/01/17/2025-01470/strengthening-and-promoting-innovation-in-the-nations-cybersecurity#p-10
    * **Publisher:** US Government
    * **License:** 
    * **Type:**  
    * **Publication date:** 2025
  </details>

### Vietnam

* [Vietnam’s Cyber Information Security Requirements for Internet of things]() - In 2021, Vietnam’s Ministry of Information and Communications issued a set of baseline cybersecurity requirements for consumer Internet-of-Things devices (for example, network cameras, Wi-Fi routers, and smart home gadgets). This was formalized in a decision (Decision 736/QD-BTTTT) that lists mandatory security features for IoT products in Vietnam. These requirements include having unique default credentials or forcing password changes on setup, providing secure update mechanisms for device firmware, implementing data protection measures, and ensuring devices undergo security testing. The regulation also often requires manufacturers to have a point of contact for vulnerability reporting. Vietnam’s move mirrors the global trend initiated by standards like ETSI EN 303 645 but makes it enforceable within the country’s jurisdiction. Manufacturers of IoT devices in Vietnam (or exporters to Vietnam) need to comply with these rules to sell their products legally. The aim is to reduce the prevalence of easily exploitable IoT devices (which could be hijacked for botnets or spying) on the Vietnamese market, thereby enhancing overall cyber hygiene and protecting consumers.
  <details>
    <summary>More info</summary>

    * **Title:** Vietnam’s Cyber Information Security Requirements for Internet of things
    * **URL:** 
    * **Publisher:** 
    * **License:** 
    * **Type:** 
    * **Publication date:** 
  </details>

## 6. Other

* [Cyber Resilience Act Requirements Standards Mapping - Joint Research Centre & ENISA Joint Analysis](https://www.enisa.europa.eu/publications/cyber-resilience-act-requirements-standards-mapping) - This joint analysis report by the European Commission’s Joint Research Centre (JRC) and ENISA examines how existing cybersecurity standards relate to the requirements of the proposed Cyber Resilience Act (CRA). The CRA will impose certain security requirements on hardware and software products in the EU, and this report maps each specific CRA requirement (for example, on secure design, vulnerability handling, encryption, etc.) to one or more international or European standards that address that topic. The analysis identifies where suitable standards already exist (and could be used to comply with or demonstrate conformity to that CRA requirement) and where there are gaps (i.e. no current standard fully covers a particular requirement, indicating a need for further standardization). This mapping is valuable for industry and regulators: manufacturers can use it to figure out which standards or certifications might help them meet CRA obligations, and standards organizations can see where new work might be needed. Overall, the report serves as a bridge between the high-level legal requirements of the CRA and the practical technical standards that can fulfill them.
  <details>
    <summary>More info</summary>

    * **Title:** Cyber Resilience Act Requirements Standards Mapping - Joint Research Centre & ENISA Joint Analysis
    * **URL:** https://www.enisa.europa.eu/publications/cyber-resilience-act-requirements-standards-mapping
    * **Publisher:** ENISA
    * **License:** 
    * **Type:** 
    * **Publication date:** 
  </details>
  
## Acknowledgments

TODO: ADD MISSING CONTRIBUTORS

The following people have contributed to this document either directly or indirectly (e.g. by raising questions):
Maxim Baele,
and Tobie Langel.

If you have contributed to this document and aren't properly acknowledged or if you want to edit or remove your name, please let us know by [opening an issue](https://github.com/orcwg/cra-hub/issues/new) and we will fix this right away.

## Annex I

Prompt used:

> I linked to a spreadsheet on google drive. These are resources that are relevant for organizations that need to adhere to the EU cyber resilience act. Add a new column "E"  in sheet 1 and insert a brief summary of the resource (1 paragraph). Do this in a dry, neutral and academic style, resembling a wikipdia summary.  all types of resources are to be taken at face value.
> 
> the url is the authorative resource. and yes the summary should reflect the content
 
LLM used: OpenAI ChatGPT 4.5 using "deep research".

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