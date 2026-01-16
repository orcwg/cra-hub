---
Status: ⚠️ Draft
guidance-id: hvac-cra-compliance-starting-points
Related issue: https://github.com/orcwg/cra-hub/issues/TBD
---

# HVAC Products and the Cyber Resilience Act (CRA)

## Introduction

HVAC (Heating, Ventilation, and Air Conditioning) systems with digital elements fall within the scope of the CRA. This includes systems with:
- Embedded software or firmware
- Network connectivity (Ethernet, Wi-Fi, cellular)
- Browser-based or web interfaces (HMI - Human-Machine Interface)
- Remote monitoring or management capabilities
- Integration with building management systems
- Cloud-based services or remote access features

As an HVAC manufacturer, you have specific obligations under [[Article 7]], [[Article 8]], and [[Article 9]] of the CRA.

## Is Your HVAC Product in Scope?

Your HVAC product is likely subject to the CRA if it:

- Contains software components (firmware, control logic, applications)
- Supports network connectivity or remote communication
- Has a web-based or browser-accessible interface for control or monitoring
- Integrates with building systems or external networks
- Relies on open source components or third-party libraries

## Product Classification: Default vs. Important

Most HVAC products with digital elements will be classified as **Important** products due to:
- Network management functionalities
- Browser-based interfaces (HMI)
- Remote access capabilities
- Building system integration potential

**Important products** have enhanced requirements for:
- Security by design ([[Article 7]])
- Documented vulnerability handling ([[Article 9]])
- Technical documentation ([[Annex I]])

See [[Article 4]] for the complete classification criteria.

## Key Compliance Areas for HVAC Manufacturers

### 1. Security by Design [[Article 7]]

Your organization must demonstrate that security is integrated throughout the product development lifecycle:

**Required Elements:**
- Documented security development processes
- Threat modeling and risk assessments
- Secure coding practices and guidelines
- Regular security testing and validation
- Documentation of security measures

**HVAC-Specific Considerations:**
- Network interface security (ports, protocols, authentication)
- Browser interface security (encryption, authentication, access control)
- Remote access implementation and protection
- Building system integration security
- Firmware update mechanisms

### 2. Vulnerability Handling [[Article 9]]

You must establish a process for identifying, assessing, and addressing security vulnerabilities:

**Required Elements:**
- Documented vulnerability handling procedures
- Timeline for vulnerability assessment (reasonably prompt)
- Process for coordinating with security researchers (responsible disclosure)
- Communication procedures for notifying customers of vulnerabilities
- Security patch development and deployment procedures

**HVAC-Specific Considerations:**
- Remote access vulnerabilities (cloud services, network management)
- HMI/browser interface vulnerabilities
- Firmware vulnerability handling and update distribution
- Legacy product support considerations
- Field deployment and customer notification strategies

### 3. Cybersecurity Assistance [[Article 8]]

You must provide customers with appropriate security-related assistance:

**Required Elements:**
- Guidance for secure deployment and configuration
- Documentation of known vulnerabilities and mitigations
- Information on security settings and options
- Regular security updates
- Support for vulnerability reporting

**HVAC-Specific Considerations:**
- Network configuration guidance (firewalls, port requirements, DHCP vs. static IP)
- HMI access security guidance (authentication, role-based access)
- Remote access security best practices
- Integration security with building management systems
- Documentation in languages and formats accessible to customers

### 4. Technical Documentation [[Annex I]]

For Important products, you must create comprehensive technical documentation including:

- Security policy and security objectives
- Information about threats and vulnerabilities relevant to the product
- Description of security measures and how they address identified threats
- Instructions for secure deployment, installation, and configuration
- Known vulnerabilities and available mitigations
- Information about security updates and how to obtain them
- Contact information for reporting vulnerabilities

## Common HVAC Security Considerations

### Network Connectivity

**Typical network interfaces in HVAC systems:**
- Local network connection (Ethernet or Wi-Fi)
- Remote management via cloud services or VPN
- Building management system integration
- Mobile app connectivity

**Security requirements:**
- Secure authentication for all network access
- Encryption of sensitive data in transit
- Firewall integration and port management guidance
- Network segmentation capabilities
- Protection against unauthorized configuration changes

### Browser-Based HMI (Web Interface)

**Common in modern HVAC systems:**
- Local browser access for technicians and operators
- Remote web-based access via cloud services
- Mobile web interfaces

**Security requirements:**
- HTTPS/TLS encryption for all communications
- Strong authentication (username/password minimum; MFA recommended)
- Session management and automatic logout
- Role-based access control (different permissions for operators vs. administrators)
- Protection against common web vulnerabilities (injection, XSS, CSRF)
- Audit logging for administrative actions

### Remote Access via Cloud Services

**Example architectures:**
- Cloud-based monitoring portal (e.g., via idcs4eu.net or similar services)
- VPN-based remote management access
- Mobile app connectivity to cloud backend

**Security requirements:**
- User authentication to the cloud service
- Data encryption in transit (HTTPS/TLS minimum)
- Encryption of sensitive data at rest
- Clear data handling and retention policies
- Compliance with privacy regulations
- Regular security assessments of cloud infrastructure

### Open Source Components

HVAC products often integrate open source libraries and components. You must:

- Maintain a bill of materials (BOM) for open source components
- Monitor for known vulnerabilities in dependencies
- Evaluate whether components meet CRA requirements
- Establish processes for security updates
- Ensure license compliance

See [[FAQ: Open Source and the CRA]] for detailed guidance.

### Firmware and Secure Updates

**HVAC-specific considerations:**
- Secure firmware update mechanisms (authenticated, encrypted)
- Rolling update strategies for devices in the field
- Rollback procedures if updates cause issues
- Support for legacy devices with older hardware constraints
- Documentation of update procedures for customers

## Compliance Timeline & Milestones

### Current Phase (Until September 2027)

**By September 12, 2027,** all "Important" products (which includes most connected HVAC systems) must:
- Be designed and developed according to CRA requirements
- Have established vulnerability handling processes
- Have documented security measures and technical documentation
- Carry CE marking indicating CRA compliance
- Not be placed on the market if non-compliant

**Recommended Timeline for HVAC Manufacturers:**

1. **Now:** Assess your products and current security practices
2. **Within 3-6 months:** Develop compliance roadmap and begin implementation
3. **6-18 months:** Implement security improvements and establish processes
4. **18-24 months:** Finalize documentation and prepare for CE marking
5. **Before September 2027:** Complete transition to compliant products

## Getting Started: Key Questions to Address

1. **Product Inventory:** Which of your HVAC products have digital elements or network connectivity?

2. **Current State:** What security development and vulnerability handling practices do you currently have in place?

3. **Network Architecture:** How do your products connect to networks? What remote access mechanisms do you support?

4. **HMI Security:** If you have browser-based interfaces, how are they currently secured?

5. **Open Source:** What open source components are integrated into your products?

6. **Resources:** What expertise and resources can you allocate to CRA compliance?

7. **Timeline:** What's your target date for achieving full compliance?

## Additional Guidance

See also:
- [[FAQ: HVAC Network Considerations]] for detailed network security requirements
- [[FAQ: Vulnerability Handling]] for establishing vulnerability management processes
- [[FAQ: Security by Design]] for integrating security into product development
- [[Questionnaire: HVAC Products]] for comprehensive compliance assessment
- [[Presentation: HVAC Products & CRA Compliance]] for consultant guidance

## Note

The CRA applies to HVAC products with digital elements, but other EU regulations may also apply depending on your specific product, customer base, and data handling practices. Consult with legal advisors familiar with EU regulations for your specific situation.
