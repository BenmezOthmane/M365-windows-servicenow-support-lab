# Hybrid Enterprise IT Operations & Service Management Lab

**ServiceNow • Microsoft 365 • Microsoft Entra ID • Active Directory • Windows • DNS • Networking**

A hands-on enterprise IT infrastructure and service management project designed, built, integrated, operated, tested, troubleshot, and documented from the ground up.

This project simulates a modern **hybrid enterprise IT environment**, combining on-premises infrastructure with Microsoft 365 cloud services and ServiceNow ITSM.

The objective is not only to demonstrate IT Support skills, but to demonstrate the ability to **design an environment, build its components, integrate services, administer systems, support users, troubleshoot technical issues, implement ITSM processes, and document the complete operational lifecycle**.

---

# 🎯 Project Overview

Modern IT environments are not built around a single technology.

A typical organization may simultaneously depend on:

* Active Directory
* Windows endpoints
* DNS
* Microsoft Entra ID
* Microsoft 365
* Exchange Online
* Microsoft Teams
* SharePoint
* OneDrive
* Network services
* ITSM platforms
* Asset and configuration management
* Service management processes

This project brings these components together into one controlled laboratory environment.

The result is a simulated enterprise environment where technical infrastructure, cloud services, users, support operations, and ITSM processes interact with each other.

---

# 🧭 Project Vision

The project follows the complete lifecycle of an IT environment:

```text
                 DESIGN
                   │
                   ▼
                 BUILD
                   │
                   ▼
                CONFIGURE
                   │
                   ▼
                INTEGRATE
                   │
                   ▼
                  TEST
                   │
                   ▼
                OPERATE
                   │
                   ▼
             TROUBLESHOOT
                   │
                   ▼
                IMPROVE
                   │
                   ▼
               DOCUMENT
```

Rather than focusing on a single role, the project demonstrates practical exposure across several areas of enterprise IT.

---

# 🏗️ Enterprise Architecture

```text
                         ┌──────────────────────────┐
                         │       ServiceNow PDI     │
                         │                          │
                         │ ITSM • CMDB • SLA        │
                         │ Incidents • Requests     │
                         │ Catalog • Knowledge      │
                         └────────────┬─────────────┘
                                      │
                              Service Management
                                      │
                ┌─────────────────────┼─────────────────────┐
                │                     │                     │
                ▼                     ▼                     ▼
        Microsoft 365          On-Premises IT          Network
                │                     │                     │
       ┌────────┼────────┐            │                     │
       │        │        │            │                     │
     Entra   Exchange  Teams        DC01                  DNS
      ID      Online                 AD DS               TCP/IP
       │        │        │            │                  Routing
       │        │        │            │                  VPN
       └────────┼────────┘            │
                │                     │
         SharePoint / OneDrive        │
                                     │
                          ┌──────────┴──────────┐
                          │                     │
                     WIN-USER-01          WIN-USER-02
                     Windows 10 Pro       Windows 10 Pro
```

---

# 🖥️ Infrastructure

## On-Premises Infrastructure

| System          | Role                                   |
| --------------- | -------------------------------------- |
| **DC01**        | Active Directory Domain Services + DNS |
| **WIN-USER-01** | Windows 10 Pro Enterprise Endpoint     |
| **WIN-USER-02** | Windows 10 Pro Enterprise Endpoint     |

The Windows endpoints represent employee workstations in the simulated organization.

They are used to demonstrate:

* Domain authentication
* User support
* Windows administration
* Application troubleshooting
* Network troubleshooting
* Group Policy-related scenarios
* Endpoint configuration
* Access troubleshooting

---

# ☁️ Cloud Infrastructure

The cloud side of the environment uses the Microsoft 365 Developer ecosystem where available.

### Microsoft Entra ID

Used for:

* Cloud identities
* Users
* Groups
* Authentication
* Access management
* Licensing
* Administrative roles
* MFA-related support
* Identity troubleshooting

### Microsoft 365

Used to simulate modern workplace services:

* Exchange Online
* Microsoft Teams
* SharePoint Online
* OneDrive
* Microsoft 365 administration

---

# 🎫 ITSM Platform

## ServiceNow

ServiceNow is the central IT Service Management platform for the project.

It represents the organization's Service Desk and service management layer.

The implementation includes:

* Incident Management
* Service Requests
* Service Catalog
* Assignment Groups
* Priorities
* SLA
* Knowledge Management
* CMDB
* Configuration Items
* User records
* Reporting
* Workflow / automation where appropriate

---

# 🧩 1. Infrastructure & Systems Design

One of the main objectives of the project is to demonstrate the ability to **design and structure an enterprise IT environment before operating it**.

The environment is designed around clear separation between:

* Identity
* Endpoints
* Cloud services
* ITSM
* Networking
* Support operations

The architecture allows technical incidents to be connected to:

```text
User
  │
  ▼
Endpoint
  │
  ▼
Identity / Network / Application
  │
  ▼
Business Service
  │
  ▼
ServiceNow Incident
```

This provides a realistic foundation for troubleshooting and service management.

---

# 🏢 2. Active Directory Administration

Active Directory provides the on-premises identity foundation.

### Implemented / Demonstrated Activities

* Domain user management
* Organizational Units
* Security groups
* Group membership
* Computer accounts
* Password management
* Account lockout investigation
* Authentication troubleshooting
* Domain joining
* Basic Group Policy troubleshooting
* Access control

### Skills Demonstrated

* Active Directory administration
* Identity management
* Access control
* Windows domain administration
* User lifecycle management

---

# 🌐 3. DNS & Network Services

DNS is treated as a core infrastructure dependency rather than simply a troubleshooting topic.

### Activities

* DNS configuration
* Name resolution
* Client DNS configuration
* Connectivity testing
* Gateway verification
* IP configuration
* Internal hostname resolution
* Network troubleshooting

### Tools

```text
ipconfig
ping
nslookup
tracert
```

Network troubleshooting follows a structured approach:

```text
Physical / Virtual Connectivity
          ↓
IP Configuration
          ↓
Gateway
          ↓
DNS Resolution
          ↓
Application Connectivity
          ↓
Service Availability
```

---

# 🪟 4. Windows Endpoint Administration

The Windows endpoints represent enterprise employee workstations.

The project demonstrates both **support and administration** capabilities.

### Endpoint Management

* Domain joining
* User profiles
* Windows configuration
* Application installation
* Windows updates
* Device Manager
* Services
* Event Viewer
* Task Manager
* PowerShell
* Command Prompt
* Windows Defender
* Printer configuration
* Network configuration

### Troubleshooting Methodology

Issues are investigated using:

```text
Identify
   ↓
Collect Evidence
   ↓
Isolate the Cause
   ↓
Apply Fix
   ↓
Validate
   ↓
Document
```

This demonstrates structured troubleshooting rather than simply applying random fixes.

---

# ☁️ 5. Microsoft Entra ID & Identity Administration

The project extends identity management from traditional Active Directory into the cloud.

### Activities

* User creation
* Group management
* Group membership
* License assignment
* Authentication troubleshooting
* MFA-related support
* Access troubleshooting
* Administrative roles
* Least-privilege principles
* Identity lifecycle management

This demonstrates understanding of the transition from traditional on-premises identity to cloud-based identity.

---

# 📧 6. Exchange Online Administration

Exchange Online is used to simulate enterprise email services.

### Activities

* Mailbox management
* Shared mailboxes
* Mailbox permissions
* Send As
* Send on Behalf
* Mail-flow troubleshooting
* Message Trace where available
* Email access investigation

The focus is on understanding the relationship between:

```text
User
 ↓
Identity
 ↓
Mailbox
 ↓
Permissions
 ↓
Mail Flow
 ↓
Business Communication
```

---

# 💬 7. Microsoft Teams Administration

Teams is used as an enterprise collaboration platform.

### Activities

* Teams creation
* Membership management
* Channel access
* User access
* Permission troubleshooting
* Collaboration support

Scenarios are designed to demonstrate how collaboration issues can originate from identity, membership, permissions or service configuration.

---

# 📁 8. SharePoint & OneDrive

Cloud file services are included as part of the modern workplace environment.

### SharePoint

* Sites
* Document libraries
* Permissions
* Sharing
* Access troubleshooting

### OneDrive

* User storage
* Synchronization
* Sharing
* Access
* Troubleshooting

The goal is to understand both the technical and support perspective of cloud file services.

---

# 🛠️ 9. ServiceNow ITSM Implementation

ServiceNow acts as the operational center of the environment.

The project demonstrates how technical work is transformed into controlled IT service processes.

---

## Incident Management

Configure and use:

* Incident categories
* Impact
* Urgency
* Priority
* Assignment Groups
* States
* Work Notes
* Customer communication
* Resolution
* Closure

Example lifecycle:

```text
New
 ↓
Assigned
 ↓
Investigating
 ↓
In Progress
 ↓
Resolved
 ↓
Closed
```

---

# 🛒 10. Service Catalog

Service Catalog is used to represent standardized employee requests.

Example services:

```text
New User Onboarding
New Device Setup
Microsoft 365 Access
Shared Mailbox Access
Teams Access
Software Installation
VPN Access
Access Change
Password Reset
```

Where appropriate, requests include:

```text
Request
   ↓
Approval
   ↓
Fulfillment
   ↓
Validation
   ↓
Closure
```

This demonstrates the difference between an **Incident** and a **Service Request**.

---

# ⏱️ 11. SLA & Service Management

SLA management is implemented to introduce service-level thinking into the environment.

Examples include:

* Response targets
* Resolution targets
* Priority-based SLAs
* Escalation
* SLA monitoring
* SLA breach scenarios

The project demonstrates how technical support is measured not only by whether an issue is solved, but also by **how effectively and within what service target it is handled**.

---

# 🗃️ 12. CMDB & Configuration Management

ServiceNow CMDB is used to represent important technology components.

Potential Configuration Items include:

```text
DC01
WIN-USER-01
WIN-USER-02
Microsoft 365 Services
Network Components
User Devices
```

Where appropriate, relationships are represented between:

```text
User
  │
  ▼
Endpoint
  │
  ▼
Service
  │
  ▼
Business Impact
```

This introduces practical Configuration Management concepts and demonstrates how infrastructure can be connected to service operations.

---

# 📚 13. Knowledge Management

A Service Desk should not solve the same problem from zero every time.

Knowledge articles are created to standardize troubleshooting and reduce repeated effort.

Examples:

```text
How to Reset a Domain Password
How to Troubleshoot DNS
How to Troubleshoot Windows Network Connectivity
How to Request Microsoft 365 Access
How to Troubleshoot OneDrive
How to Resolve Teams Access Issues
```

Articles contain:

* Symptoms
* Possible causes
* Troubleshooting steps
* Resolution
* Validation
* Escalation criteria

---

# 👤 14. User Lifecycle & Onboarding

The project demonstrates a simplified enterprise employee lifecycle.

```text
New Employee
     │
     ▼
ServiceNow Request
     │
     ▼
Approval
     │
     ├───────────────┐
     ▼               ▼
Active Directory   Microsoft 365
     │               │
     ▼               ▼
Windows Device    Cloud Services
     │               │
     └───────┬───────┘
             ▼
       User Ready
```

This demonstrates interaction between:

* Service Desk
* Identity
* Active Directory
* Microsoft 365
* Windows
* Access Management
* ITSM

---

# 🔄 15. Integration Between Systems

The value of the project comes from connecting the individual technologies into one operational model.

Instead of treating every technology independently:

```text
Active Directory
Microsoft 365
Windows
Networking
ServiceNow
```

they are treated as components of the same enterprise environment.

For example:

```text
Employee
   │
   ├── AD Account
   │
   ├── Microsoft 365 Identity
   │
   ├── Windows Endpoint
   │
   ├── Teams / Exchange / OneDrive
   │
   └── ServiceNow User / Requests / Incidents
```

This provides a more realistic representation of enterprise IT operations.

---

# 🚨 16. Technical Incident & Support Scenarios

This project deliberately avoids simply reproducing the ten common incidents already implemented in the previous GLPI project.

The previous project established the foundation of traditional ITSM and support operations.

This project expands that foundation into **cloud, identity, enterprise administration and integrated IT operations**.

Potential scenarios include:

### Identity

* MFA registration problem
* Microsoft 365 sign-in issue
* License assignment problem
* Entra ID access problem
* Group-based access problem

### Exchange Online

* Send As permission problem
* Shared mailbox access workflow
* Mail-flow investigation

### Teams

* Team membership problem
* Access/permission issue
* Collaboration configuration issue

### SharePoint / OneDrive

* SharePoint permission issue
* File access problem
* Sharing configuration issue
* Cloud synchronization problem

### Windows / Infrastructure

* Domain authentication problem
* Group Policy issue
* Windows service failure
* Application configuration issue
* Network connectivity problem

### ServiceNow

* Service Catalog request
* Approval workflow
* SLA escalation
* SLA breach
* CMDB relationship
* User onboarding workflow

The final scenarios will be selected according to the capabilities actually available in the lab.

---

# 🧪 17. Testing & Validation

Every major implementation should be validated rather than assumed to be working.

Testing includes:

```text
Configuration
      ↓
Functional Test
      ↓
Negative Test
      ↓
Troubleshooting
      ↓
Validation
      ↓
Evidence
```

Examples:

* Test user authentication
* Test group-based access
* Test DNS resolution
* Test domain connectivity
* Test Microsoft 365 access
* Test ServiceNow ticket lifecycle
* Test Service Catalog requests
* Test SLA behavior
* Test CMDB relationships

---

# 📊 18. Documentation & Evidence

The project is documented as an operational portfolio rather than simply a collection of screenshots.

Evidence includes:

### ServiceNow

```text
Incidents
Requests
Service Catalog
CMDB
SLA
Knowledge Base
Assignment Groups
Reports
```

### Microsoft 365

```text
Entra ID
Users
Groups
Licenses
Exchange Online
Teams
SharePoint
OneDrive
```

### Windows

```text
System Configuration
Event Viewer
Task Manager
Services
Device Manager
PowerShell
Network Configuration
```

### Infrastructure

```text
Active Directory
DNS
Domain Configuration
Network Testing
```

---

# 📂 Repository Structure

```text
m365-windows-servicenow-support-lab/
│
├── README.md
│
├── docs/
│   ├── architecture/
│   ├── implementation/
│   ├── troubleshooting/
│   └── procedures/
│
├── incidents/
│   ├── identity/
│   ├── microsoft365/
│   ├── windows/
│   ├── network/
│   └── servicenow/
│
├── requests/
│   ├── onboarding/
│   ├── access/
│   └── software/
│
├── knowledge-base/
│
├── screenshots/
│   ├── servicenow/
│   ├── microsoft365/
│   ├── windows/
│   └── network/
│
└── assets/
    └── diagrams/
```

---

# 🧠 Skills Demonstrated

## IT Support & Service Desk

* Incident Management
* Service Requests
* User Support
* Troubleshooting
* Escalation
* Knowledge Management
* Documentation
* Customer-oriented support

## Systems Administration

* Active Directory
* Windows administration
* User management
* Groups
* Domain services
* DNS
* Endpoint troubleshooting
* PowerShell
* Basic Group Policy troubleshooting

## Microsoft 365 / Cloud

* Microsoft Entra ID
* Identity management
* Microsoft 365 administration
* Exchange Online
* Microsoft Teams
* SharePoint
* OneDrive
* Access management
* Cloud troubleshooting

## ITSM / Service Management

* ServiceNow
* Incident Management
* Service Requests
* Service Catalog
* SLA
* CMDB
* Configuration Items
* Knowledge Management
* Assignment Groups
* Service workflows
* Reporting

## Infrastructure

* Enterprise architecture concepts
* Client/server architecture
* Hybrid IT concepts
* DNS
* TCP/IP
* Network troubleshooting
* Identity infrastructure
* Endpoint infrastructure

---

# 👨‍💻 Roles Simulated

Through this project, multiple aspects of enterprise IT roles are practically demonstrated.

### IT Support / Service Desk

Handling:

* Incidents
* Requests
* User problems
* Troubleshooting
* Escalation
* Documentation

### Desktop / Endpoint Support

Managing:

* Windows endpoints
* Applications
* Devices
* User environments
* Connectivity

### Junior Systems Administration

Working with:

* Active Directory
* DNS
* Users
* Groups
* Domain infrastructure
* Windows systems

### Microsoft 365 / Cloud Administration

Working with:

* Entra ID
* Exchange Online
* Teams
* SharePoint
* OneDrive

### ITSM / ServiceNow Administration

Working with:

* Incidents
* Requests
* Catalog
* SLA
* CMDB
* Knowledge
* Assignment Groups

### Infrastructure / Systems Design

Designing and connecting the components into a coherent enterprise environment.

The project does **not** claim production-level expertise in every one of these disciplines. Instead, it demonstrates hands-on exposure and practical implementation across the technologies that interact in a modern enterprise IT environment.

---

# 💰 Cost Strategy

The project is designed to operate with **zero or minimal cost**.

Primary resources:

* ServiceNow Personal Developer Instance
* Microsoft 365 Developer Program, where eligible
* Existing VMware infrastructure
* Existing Windows systems
* Existing Active Directory environment
* GitHub for documentation

The environment is intended strictly for:

* Learning
* Development
* Testing
* Demonstration
* Portfolio purposes

No production infrastructure is required.

---

# 📈 Project Philosophy

The project follows several principles:

### 1. Build before documenting

The environment should be genuinely implemented before claiming completion.

### 2. Test before claiming success

Every important component should have evidence of successful operation.

### 3. Troubleshoot like a real IT environment

Problems are investigated systematically instead of simply reinstalling components.

### 4. Connect technologies together

The goal is to understand how enterprise systems depend on each other.

### 5. Document the entire lifecycle

Architecture, implementation, configuration, testing, troubleshooting and results are documented.

### 6. Demonstrate capability, not just tool familiarity

The objective is not to show that a product was opened.

The objective is to show that it was **used to solve realistic enterprise problems**.

---

# 🚀 Project Status

* [x] Existing AD/DNS infrastructure available
* [x] Windows endpoints available
* [ ] ServiceNow PDI
* [ ] ServiceNow foundation
* [ ] ServiceNow users and groups
* [ ] Incident Management
* [ ] Service Catalog
* [ ] CMDB
* [ ] SLA
* [ ] Knowledge Base
* [ ] Microsoft 365 Developer environment
* [ ] Entra ID
* [ ] Exchange Online
* [ ] Teams
* [ ] SharePoint
* [ ] OneDrive
* [ ] Integration testing
* [ ] New technical scenarios
* [ ] Evidence collection
* [ ] Final documentation
* [ ] LinkedIn project presentation

---

# 🏁 Final Outcome

The final result will be a complete simulated **Hybrid Enterprise IT Operations environment**.

The project demonstrates the ability to move through the full lifecycle:

```text
                ┌──────────────┐
                │   DESIGN     │
                └──────┬───────┘
                       ▼
                ┌──────────────┐
                │    BUILD     │
                └──────┬───────┘
                       ▼
                ┌──────────────┐
                │  CONFIGURE   │
                └──────┬───────┘
                       ▼
                ┌──────────────┐
                │  INTEGRATE   │
                └──────┬───────┘
                       ▼
                ┌──────────────┐
                │     TEST     │
                └──────┬───────┘
                       ▼
                ┌──────────────┐
                │    OPERATE   │
                └──────┬───────┘
                       ▼
                ┌──────────────┐
                │ TROUBLESHOOT │
                └──────┬───────┘
                       ▼
                ┌──────────────┐
                │  DOCUMENT    │
                └──────────────┘
```

The project therefore goes beyond demonstrating basic IT Support.

It demonstrates practical exposure to **IT Operations, Systems Administration, Microsoft 365 Administration, Identity & Access Management, Windows Endpoint Management, Networking, ITSM, ServiceNow, Configuration Management, Service Management, troubleshooting, integration and technical documentation**.

The central objective is to demonstrate not only:

> **"I can support an IT environment."**

but also:

> **"I can design it, build it, configure it, integrate its components, operate it, troubleshoot it, manage its services, and document what I implemented."**
