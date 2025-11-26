---
title: "Device management"
weight: 020
description: "This section describes the configuration of endpoint device management settings within Microsoft Defender associated with systems built according to the guidance provided by ASD's Blueprint for Secure Cloud."
---

{{% alert title="Instruction" color="dark" %}}

The below tables outline the _as built_ configuration for ASD's _Blueprint for Secure Cloud_ (the Blueprint) for the Microsoft Defender portal at the following URL:

<https://security.microsoft.com/securitysettings/endpoints/onboarding>

The settings described on these pages provide a baseline implementation for a system configured using the Blueprint. Any implementation implied by these pages should not be considered as prescriptive as to how an organisation must scope, build, document, or assess a system.

Implementation of the guidance provided by the Blueprint will differ depending on an organisation’s operating context and organisational culture. Organisations should implement the Blueprint in alignment with their existing change management, business processes and frameworks.

Placeholders such as `<ORGANISATION.GOV.AU>`, `<BLUEPRINT.GOV.AU>` and `<TENANT-NAME>` should be replaced with the relevant details as required.

{{% /alert %}}

### Onboarding

| Item                                                |                                       Value |
| --------------------------------------------------- | ------------------------------------------: |
| Select operating system to start onboarding process |                           Windows 10 and 11 |
| Connectivity type                                   |                                 Streamlined |
| Deployment method                                   | Mobile Device Management / Microsoft Intune |

### Offboarding

| Item                                                 |                                       Value |
| ---------------------------------------------------- | ------------------------------------------: |
| Select operating system to start offboarding process |                           Windows 10 and 11 |
| Deployment method                                    | Mobile Device Management / Microsoft Intune |

### Related information

#### Security and governance

- [Essential Eight - Patch applications](/security-and-governance/essential-eight/patch-applications)
- [Essential Eight - Patch operating systems](/security-and-governance/essential-eight/patch-os)

#### Design

- [Endpoints and devices](/design/platform/security/endpoint-security)

#### Configuration

- [Networking](/configuration/networking)

#### References

- [Onboard devices to Microsoft Defender for Endpoint](https://learn.microsoft.com/en-au/defender-endpoint/onboarding)
- [Offboard devices](https://learn.microsoft.com/en-au/defender-endpoint/offboard-machines)
