# Questionnaire for HVAC manufacturers in terms of the CRA

## Introduction

Digital elements in HVAC (Heating, Ventilation, and Air Conditioning) systems fall under the scope of the CRA. This includes:
- Network connectivity and remote management capabilities
- Browser-based or web interfaces (HMI - Human Machine Interface)
- Building management system integrations
- Cloud-based services and remote monitoring
- Firmware and embedded software components

This questionnaire helps HVAC manufacturers assess their CRA compliance readiness and identify key areas requiring attention.

## Product Architecture & Connectivity

* Does your HVAC product contain digital elements or software components?
  * If yes, are they integrated into the product or sold separately?

* Does your HVAC system support network connectivity?
  * If yes, what types of network interfaces are supported (Ethernet, Wi-Fi, cellular, other)?

* Does your HVAC product feature a browser-based or web interface (HMI) for control and monitoring?
  * If yes, what are the primary use cases (local control, remote access, building integration)?

* Does your HVAC system support remote access capabilities?
  * If yes, is remote access enabled through:
    * Direct cloud services?
    * Third-party cloud platforms?
    * VPN or secure tunnels?
    * Other methods?

* What remote access ports and protocols does your system use?
  * Examples: port 21/TCP (FTP), 5900/TCP (VNC), 40961/TCP (remote management), HTTPS, SSH, other?

* Does your HVAC product integrate with building management systems (BMS) or other building systems?
  * If yes, what protocols and interfaces are used?

## Current Security Posture

* Does your organization have existing security practices in place for your HVAC products?
  * If yes, please describe your approach to:
    * Security by design and development
    * Vulnerability identification and response
    * Security testing and validation
    * Documentation and traceability

* How do you currently handle vulnerability reports from customers, researchers, or other parties?
  * Do you have a documented vulnerability handling process?
  * Do you have a security point of contact or CSIRT?

* Do you currently conduct security assessments or penetration testing of your HVAC products?
  * If yes, how frequently and what scope?

* Are there specific security risks you see in your HVAC products that concern you?
  * (e.g., unauthorized remote access, network exposure, firmware tampering, integration vulnerabilities)

## Network Configuration & Connectivity

* How is your HVAC product typically configured for network connectivity?
  * Dynamic IP assignment via DHCP?
  * Static IP configuration?
  * Automatic network detection and configuration?

* What network security measures are currently implemented?
  * Firewall integration or built-in firewall?
  * Network segmentation capabilities?
  * Authentication mechanisms for network access?
  * Encryption of network communications?

* If your HVAC system supports remote access, what security measures protect that connection?
  * Examples: certificate validation, authentication tokens, rate limiting, access control?

* Are there specific ports or services that must be open for your HVAC system to function?
  * If yes, which ones and why?

* Do you provide guidance to customers on firewall configuration or network security best practices?

* Does your HVAC system support DNS configuration or resolution?
  * If yes, do customers control this, or is it managed by the manufacturer?

## Browser/Web Interface (HMI) & Remote Access

* Describe the technical architecture of your HVAC HMI or web interface:
  * Is it a browser-based application (accessed via HTTP/HTTPS)?
  * Is it a standalone application (installed on a computer or mobile device)?
  * Is it both?

* What technologies are used to build the HMI?
  * (e.g., HTML/CSS/JavaScript, specific frameworks, proprietary protocols)

* How is the HMI accessed by users?
  * Local network access only?
  * Remote access via cloud services?
  * Remote access via VPN?
  * Other methods?

* If remote access is supported, describe the security implementation:
  * How is authentication handled (username/password, multi-factor, single sign-on)?
  * Is communication encrypted (HTTPS, TLS)?
  * Are there rate limiting or brute-force protections?
  * How are sessions managed and terminated?

* Do you use cloud services for remote access or monitoring?
  * If yes, which services or providers?
  * What data is transmitted to the cloud?
  * How is data protected in transit and at rest?

* Does your HMI support integration with third-party systems or APIs?
  * If yes, how is that integration secured?

* Are there different user roles or permission levels in your HMI?
  * If yes, how are permissions enforced and managed?

## Open Source Dependencies

* What open source components or libraries are integrated into your HVAC products?
  * For critical components, do you maintain a bill of materials (BOM)?

* Do you monitor open source components for known vulnerabilities?
  * If yes, what tools or processes do you use?

* How do you manage updates to open source components?
  * Do you apply security patches promptly?
  * What is your testing process for updates?

* Have you assessed whether your open source components meet CRA requirements?
  * If not, what are the barriers to doing so?

* Do you contribute back to open source projects you depend on?
  * If yes, in what ways (bug reports, patches, funding, other)?

* What support or resources would help you ensure your open source components comply with the CRA?

* Are you aware of the licenses used by your open source components?
  * Do you have processes to ensure license compliance in your products?

* Do you have a backup plan if critical open source projects you depend on are abandoned?

## Vulnerability Handling & Security Updates

* How do you notify customers of security vulnerabilities or updates?
  * (e.g., email, security advisories, product notifications)

* What is your typical timeline for releasing security patches after vulnerability discovery?
  * Can you support older versions with security patches, or do you require upgrades?

* Do you have a process for coordinating with security researchers before public disclosure?
  * Do you have a responsible disclosure policy?

* How do customers apply updates to your HVAC products?
  * Over-the-air (OTA) updates?
  * Manual firmware updates?
  * Automatic updates?

* Do you monitor your products in the field for security issues or attacks?
  * If yes, how do you respond to detected issues?

## CRA Compliance Readiness

* What is your current understanding of CRA requirements as they apply to your products?

* What timeline are you targeting for CRA compliance?

* Have you assessed whether your HVAC products fall under the "Important" product category?
  * (Products with network management functionalities or browser-based interfaces are likely Important)

* What resources or expertise would your organization need to achieve CRA compliance?
  * (e.g., security expertise, legal guidance, compliance tools, training)

* What aspects of CRA compliance do you view as most challenging for HVAC products?

* Is there specific guidance or support you need regarding:
  * Security by design requirements?
  * Vulnerability handling processes?
  * Documentation and CE marking?
  * Network security for HVAC systems?
  * HMI/browser interface security?

* Are you already collaborating with cybersecurity experts or compliance consultants?
  * If yes, in what capacity?

* Do you see opportunities for industry collaboration on CRA compliance among HVAC manufacturers?

## Next Steps

This questionnaire is designed to help identify your organization's CRA compliance readiness and specific guidance needs. Your responses will inform:

- Customized compliance roadmaps for your products
- Identification of priority areas for remediation
- Recommendations for security improvements
- Potential collaboration opportunities with other manufacturers or industry groups

Please return completed questionnaires to [contact information].
