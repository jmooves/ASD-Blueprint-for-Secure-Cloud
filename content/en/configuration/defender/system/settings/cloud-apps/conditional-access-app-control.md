---
title: "Conditional Access App Control"
weight: 010
description: "This section describes the configuration of Conditional Access App Control settings within Microsoft Defender associated with systems built according to the guidance provided by ASD's Blueprint for Secure Cloud."
---

{{% alert title="Instruction" color="dark" %}}

The below tables outline the _as built_ configuration for ASD's _Blueprint for Secure Cloud_ (the Blueprint) for the Microsoft Defender portal at the following URL:

<https://security.microsoft.com/cloudapps/settings?tabid=proxyHardening>

The settings described on these pages provide a baseline implementation for a system configured using the Blueprint. Any implementation implied by these pages should not be considered as prescriptive as to how an organisation must scope, build, document, or assess a system.

Implementation of the Blueprint will differ depending on an organisation’s operating context and organisational culture. Organisations should implement the Blueprint in alignment with their existing change management, business processes and frameworks.

Placeholders such as `<ORGANISATION.GOV.AU>`, `<BLUEPRINT.GOV.AU>` and `<TENANT-NAME>` should be replaced with the relevant details as required.

{{% /alert %}}

### Default behavior

| Item                                     |        Value |
| ---------------------------------------- | -----------: |
| Default behavior during system downtime: | Allow access |

### User monitoring

| Item                                                |               Value |
| --------------------------------------------------- | ------------------: |
| Notify users that their activity is being monitored | Use default message |

### Related information

#### Security and governance

- [Essential Eight - Application control](/security-and-governance/essential-eight/application-control)
- [System management](/security-and-governance/system-security-plan/system-management)

#### Design

- [Entra ID Protection](/design/platform/identity/protection)

#### Configuration

- [Entra ID Protection](/configuration/entra-id/protection)
- [Endpoint security](/configuration/intune/endpoint-security)

#### References

- None identified
