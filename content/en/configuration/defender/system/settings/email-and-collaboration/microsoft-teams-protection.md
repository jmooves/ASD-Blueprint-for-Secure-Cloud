---
title: "Microsoft Teams protection"
weight: 010
description: "This section describes the configuration of Teams protection settings within Microsoft Defender associated with systems built according to the guidance provided by ASD's Blueprint for Secure Cloud."
---

{{% alert title="Instruction" color="dark" %}}

The below tables outline the _as built_ configuration for ASD's _Blueprint for Secure Cloud_ (the Blueprint) for the Microsoft Defender portal at the following URL:

<https://security.microsoft.com/securitysettings/teamsProtectionPolicy>

The settings described on these pages provide a baseline implementation for a system configured using the Blueprint. Any implementation implied by these pages should not be considered as prescriptive as to how an organisation must scope, build, document, or assess a system.

Implementation of the guidance provided by the Blueprint will differ depending on an organisation’s operating context and organisational culture. Organisations should implement the Blueprint in alignment with their existing change management, business processes and frameworks.

Placeholders such as `<ORGANISATION.GOV.AU>`, `<BLUEPRINT.GOV.AU>` and `<TENANT-NAME>` should be replaced with the relevant details as required.

{{% /alert %}}

### Microsoft Teams protection

| Item                       | Value |
| -------------------------- | ----: |
| Zero-hour auto purge (ZAP) |    On |

#### Quarantine policies

| Item                     |                         Value |
| ------------------------ | ----------------------------: |
| Malware                  | Quarantine policy<sup>1</sup> |
| High-confidence phishing | Quarantine policy<sup>1</sup> |

1: [Quarantine policies](/configuration/defender/email-and-collaboration/policies-and-rules/threat-policies/quarantine-policy/quarantine-policy) may need creating prior to using them with ZAP.

#### Exclude these participants

| Item    |  Value |
| ------- | -----: |
| Users   | _None_ |
| Groups  | _None_ |
| Domains | _None_ |

### Related information

#### Security and governance

- None identified

#### Design

- [Teams clients](/design/endpoints/applications/teams-clients)

#### Configuration

- [Quarantine policy](/configuration/defender/email-and-collaboration/policies-and-rules/threat-policies/quarantine-policy/quarantine-policy)

#### References

- [Zero-hour auto purge (ZAP) in Microsoft Teams](https://learn.microsoft.com/en-au/defender-office-365/zero-hour-auto-purge#zero-hour-auto-purge-zap-in-microsoft-teams)
