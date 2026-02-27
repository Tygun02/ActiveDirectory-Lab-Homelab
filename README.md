# Active Directory Homelab – Windows Server 2022

Enterprise-style Active Directory homelab built to simulate a small business Windows domain environment.

This lab demonstrates hands-on configuration, administration, and troubleshooting of Active Directory Domain Services (AD DS), DNS, DHCP, Group Policy, and PowerShell automation.

---

## Lab Environment

**Host Machine**
- VMware Workstation
- Windows 11 Host

**Virtual Machines**
- Windows Server 2022 (Domain Controller)
- Windows 11 Pro (Domain-Joined Client)

**Domain Name**
- LAB.local
  
## Lab Architecture Diagram

![Lab Architecture](docs/images/Active-Directory-Homelab-Architecture.svg)
---

## Core Components Implemented

- Active Directory Domain Services (AD DS)
- DNS Server configuration
- DHCP configuration and scope management
- Organizational Unit (OU) design
- User and Group provisioning
- Group Policy Object (GPO) deployment
- Domain join configuration
- Remote Desktop configuration
- PowerShell-based administrative automation

---

## Skills Demonstrated

### Identity & Access Management
- User account creation and management
- Security group configuration
- OU structuring based on business model
- Delegation concepts

### Group Policy Management
- GPO creation and linking
- Local administrator policy control
- RDP restriction policy
- Policy validation using `gpresult`

### Networking Services
- DNS zone configuration
- Forwarders setup
- DHCP scope configuration
- IP lease management

### Troubleshooting
- Domain join failures
- GPO application issues
- DNS resolution errors
- User authentication problems
- RDP access control issues

---

## PowerShell Automation

- Bulk user creation scripts
- Administrative task scripting
- Robocopy-based backup scripting

---

## Validation & Testing

Each configuration was validated using:

- `gpresult /r`
- Event Viewer logs
- DNS resolution testing (`nslookup`)
- RDP connection testing
- User login verification

Screenshots and evidence are stored within the repository.

---

## Purpose of This Lab

This homelab was built to simulate real-world Help Desk and Junior System Administrator scenarios, focusing on:

- Structured troubleshooting
- Documentation discipline
- Secure configuration practices
- Enterprise-style domain management

---

## Future Improvements

- Additional GPO security hardening
- Azure AD hybrid integration
- Backup and recovery scenario simulation
- Advanced PowerShell automation

---

**Location:** Netherlands  
**Role Target:** IT Support / Help Desk / Junior System Administrator
