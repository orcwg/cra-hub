---
Status: ⚠️ Draft
guidance-id: hvac-network-considerations
Related issue: https://github.com/orcwg/cra-hub/issues/TBD
---

# HVAC Network Compliance Considerations

## Overview

Network connectivity is a critical aspect of HVAC system compliance under the CRA. This guidance addresses the security requirements for network interfaces, remote access, and integration with building systems.

## Network Interface Configuration

### DHCP vs. Static IP Assignment

**DHCP (Dynamic Host Configuration Protocol):**
- Automatic IP address assignment
- Simplifies deployment in diverse network environments
- Requires secure DHCP server implementation
- Ensure the HVAC system validates DHCP responses

**Static IP Configuration:**
- Fixed IP address configured at installation
- Requires manual configuration by technician
- More predictable for network management
- Document static IP range requirements

**Security Requirement:**
Your system must support secure IP configuration and must not expose sensitive management functions through default or easily guessable addresses. Provide customers with clear guidance on secure configuration options.

### DNS Configuration

HVAC systems often require DNS resolution for:
- Cloud service connectivity
- Building management system communication
- Firmware update servers
- Remote monitoring platforms

**Configuration Options:**
1. **Customer-Controlled DNS:**
   - Customers configure DNS servers (DHCP or static)
   - Allows network segregation and filtering
   - Requires robust handling of DNS failures
   - Document recommended DNS security practices

2. **Manufacturer-Provided DNS:**
   - Factory-configured DNS servers
   - Ensure encrypted DNS queries (DNSSEC, DNS over HTTPS)
   - Publish DNS configuration clearly
   - Provide override mechanism for customer networks

**Security Requirements:**
- Document DNS configuration approach
- Protect DNS queries from eavesdropping
- Handle DNS resolution failures gracefully
- Warn users about DNS hijacking risks
- Support split-DNS configurations for building networks

### Firewall Integration & Port Management

HVAC systems must be compatible with customer firewall policies. Key considerations:

#### Essential Ports (Must Be Open)

Document and justify every port required for operation:

**Port 21/TCP - FTP (File Transfer Protocol):**
- Legacy file transfer for firmware updates or log retrieval
- **Security Risk:** FTP credentials transmitted in plaintext
- **Recommendation:** Deprecate FTP; migrate to SFTP or HTTPS
- **If Still Required:** Restrict to local network only, document as deprecated, plan removal timeline

**Port 5900/TCP - VNC (Virtual Network Computing):**
- Remote desktop access for remote technician support
- **Security Risk:** VNC is vulnerable to several attacks without proper implementation
- **Requirements:**
  - Use secure VNC implementation with strong authentication
  - Require HTTPS/TLS tunneling for remote VNC access
  - Implement rate limiting for failed authentication attempts
  - Document that remote VNC access requires additional security measures
  - Provide alternative secure remote access methods when possible

**Port 40961/TCP - Remote Management:**
- Custom remote management protocol
- **Requirements:**
  - Implement strong mutual authentication (client and server verify each other)
  - Encrypt all traffic (HTTPS/TLS minimum, consider additional encryption)
  - Implement access controls and audit logging
  - Document the protocol and security measures
  - Provide customer guidance on secure deployment

**Port 443/TCP - HTTPS (Web Interface/HMI):**
- Browser-based interface for control and monitoring
- **Requirements:**
  - Use current TLS version (1.2 minimum, 1.3 recommended)
  - Implement strong authentication
  - Protect against common web vulnerabilities
  - Document security features and configuration options

#### Optional/Conditional Ports

Clearly document any ports that are optional or environment-specific:
- Cloud service connectivity (specific to your cloud provider)
- Building management system integration
- Mobile app connectivity
- Diagnostic or logging services

**Customer Guidance:**
Provide customers with:
- Clear list of all ports used by your HVAC system
- Purpose and security considerations for each port
- Whether each port is required, optional, or deprecated
- Recommended firewall rules for each port
- Alternative secure methods when available

### Network Segmentation & Isolation

**Recommendations for HVAC System Deployment:**

1. **Isolated Network Segment:**
   - Deploy HVAC system on dedicated network segment or VLAN
   - Separate from general building network if possible
   - Implement firewall rules between segments

2. **DMZ Deployment (For Remote Access):**
   - If supporting remote access via cloud service
   - Consider placing remote access gateway in DMZ
   - Restrict direct access from building network to HVAC system

3. **Documentation:**
   - Provide network segmentation guidance to customers
   - Explain security benefits of isolation
   - Document integration points with other building systems
   - Recommend security configurations for building networks

## Remote Access Security

### Cloud Service Integration (Example: idcs4eu.net)

Many HVAC manufacturers use cloud services for remote monitoring and management:

**Architecture:**
- HVAC system initiates outbound connection to cloud service
- Technicians access HVAC system through cloud portal/application
- System sends telemetry and monitoring data to cloud

**Security Requirements:**

**1. Authentication:**
- Authenticate HVAC systems to the cloud service (certificate-based or strong credentials)
- Authenticate users to the cloud service (strong passwords, MFA recommended)
- Document authentication mechanisms

**2. Encryption:**
- Encrypt all communication between HVAC system and cloud (HTTPS/TLS minimum)
- Encrypt sensitive data at rest in the cloud
- Protect cloud API credentials from exposure
- Document encryption implementation

**3. Data Handling:**
- Define what data is collected and sent to cloud
- Document data retention policies
- Provide customers with data deletion options
- Document compliance with privacy regulations
- Implement access controls for sensitive data in the cloud

**4. Cloud Provider Assessment:**
- Evaluate security posture of cloud provider
- Document provider's security certifications
- Implement contractual requirements for data protection
- Establish incident response procedures with cloud provider

**5. Fallback Procedures:**
- Document what happens if cloud service is unavailable
- Ensure local operation is possible without cloud connectivity
- Provide backup access methods for technicians
- Test failover scenarios regularly

### VPN-Based Remote Access

**Architecture:**
- Technicians connect via VPN to building network
- VPN gateway provides access to local HVAC management interface

**Security Requirements:**

1. **VPN Implementation:**
   - Use strong VPN protocols (IKEv2/IPsec or OpenVPN with modern TLS)
   - Implement client certificate authentication
   - Support multi-factor authentication
   - Document VPN configuration and requirements

2. **Access Control:**
   - Implement role-based access control for VPN users
   - Log all VPN connections and actions
   - Implement timeout and session management
   - Restrict VPN access to authorized technicians only

3. **Documentation:**
   - Provide customers with VPN setup and security guidance
   - Document recommended VPN configurations
   - Explain firewall requirements for VPN gateway
   - Provide security best practices for administrators

## HMI/Web Interface & Network Security

### HTTPS/TLS Requirements

**Minimum Requirements:**
- Use TLS 1.2 or higher (TLS 1.3 recommended)
- Use strong cipher suites (no RC4, DES, or other weak ciphers)
- Implement HSTS (HTTP Strict-Transport-Security) headers
- Validate server certificates properly on client side

**Certificate Management:**
- Use valid, properly signed certificates from recognized CAs
- Implement automatic certificate renewal before expiration
- Support certificate pinning if appropriate for your deployment
- Document certificate management procedures

### Authentication & Authorization

**User Authentication:**
- Require strong authentication for all access (username/password minimum)
- Implement account lockout after failed attempts
- Support multi-factor authentication for remote access
- Document password requirements and best practices

**Authorization & Roles:**
- Implement role-based access control
- Define different permission levels (operator, technician, administrator)
- Document what actions each role can perform
- Implement least-privilege access principle

**Session Management:**
- Implement secure session tokens (not user IDs or predictable values)
- Set appropriate session timeouts
- Implement automatic logout on inactivity
- Prevent session fixation and hijacking attacks

### Audit Logging

**What to Log:**
- All user authentication attempts (successes and failures)
- All administrative actions and configuration changes
- All access to sensitive data or functions
- All system and security events

**Log Protection:**
- Protect logs from unauthorized modification
- Implement log retention policies
- Archive logs securely for compliance requirements
- Document how to access and review logs

## Network Monitoring & Security

### Customer Guidance

Provide customers with recommendations for:

1. **Network Monitoring:**
   - Monitor HVAC system network traffic for anomalies
   - Implement intrusion detection if available
   - Review access logs regularly
   - Alert on suspicious activity

2. **Firewall Configuration:**
   - Recommend specific firewall rules for your HVAC system
   - Document port requirements and justify each one
   - Explain the purpose and security risk of each port
   - Suggest closing or restricting non-essential ports

3. **Network Security:**
   - Recommend network segmentation
   - Explain the benefit of isolated VLAN for HVAC systems
   - Document building management system integration requirements
   - Provide guidance on secure wireless network deployment

### Manufacturer Responsibility

You must:
- Document all network communication and protocols
- Identify and justify all required ports
- Provide secure alternatives where possible (e.g., SFTP instead of FTP)
- Support customer security requirements and filtering
- Be responsive to security vulnerabilities in network protocols

## Technical Documentation Requirements

Your [[Annex I]] technical documentation must include:

1. **Network Architecture Diagram:**
   - Show how the HVAC system connects to networks
   - Document all network interfaces and protocols
   - Show integration points with building systems
   - Identify trust boundaries

2. **Network Security Measures:**
   - Describe authentication mechanisms
   - Document encryption implementation
   - Explain access controls
   - Document logging and monitoring capabilities

3. **Configuration Guidance:**
   - Provide step-by-step instructions for secure network configuration
   - Document DHCP vs. static IP options
   - Explain DNS configuration options
   - Provide firewall rule templates or recommendations

4. **Port and Protocol Documentation:**
   - List all ports used (required, optional, deprecated)
   - Document the purpose of each port
   - Explain security implications
   - Provide recommended firewall configurations

5. **Vulnerability Information:**
   - Document known vulnerabilities related to network access
   - Explain mitigations and workarounds
   - Provide timeline for security updates
   - Explain how to obtain and apply updates

## Compliance Checklist

**Network Configuration:**
- ☐ Documented all network interfaces and connectivity methods
- ☐ Identified all required ports and justified each one
- ☐ Provided secure alternatives to legacy protocols (FTP, unencrypted access)
- ☐ Documented DHCP and static IP configuration options
- ☐ Provided DNS configuration guidance and security recommendations
- ☐ Supported firewall integration and network segmentation

**Remote Access Security:**
- ☐ Implemented strong authentication for all remote access
- ☐ Encrypted all remote access traffic (HTTPS/TLS minimum)
- ☐ Documented cloud service integration and security measures
- ☐ Implemented fallback procedures if cloud service is unavailable
- ☐ Provided customer guidance for secure remote access deployment
- ☐ Identified and addressed known vulnerabilities in remote access

**HMI/Web Interface:**
- ☐ Implemented HTTPS/TLS with strong cipher suites
- ☐ Implemented strong user authentication
- ☐ Implemented role-based access control
- ☐ Implemented audit logging for all actions
- ☐ Protected sessions from hijacking and fixation
- ☐ Documented all security features and configuration options

**Documentation:**
- ☐ Provided complete network architecture documentation
- ☐ Documented all security measures
- ☐ Provided secure configuration guidance
- ☐ Documented all known vulnerabilities and mitigations
- ☐ Explained how to obtain security updates

## See Also

- [[FAQ: HVAC CRA Compliance Starting Points]] for general HVAC CRA overview
- [[FAQ: Security by Design]] for product security development requirements
- [[FAQ: Vulnerability Handling]] for security vulnerability procedures
- [[Questionnaire: HVAC Products]] for comprehensive compliance assessment
