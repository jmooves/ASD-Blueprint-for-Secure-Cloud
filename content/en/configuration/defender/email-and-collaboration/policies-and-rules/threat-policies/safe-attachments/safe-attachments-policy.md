---
title: "Safe links policy"
weight: 010
description: "This section describes the configuration of the safe attachments policy settings within Microsoft Defender associated with systems built according to the guidance provided by ASD's Blueprint for Secure Cloud."
---

{{% alert title="Instruction" color="dark" %}}

The below pages outline the _as built_ configuration for ASD's _Blueprint for Secure Cloud_ (the Blueprint) for the Microsoft Defender portal at the following URL:

<https://security.microsoft.com/safelinksv2>

The settings described on these pages provide a baseline implementation for a system configured using the Blueprint. Any implementation implied by these pages should not be considered as prescriptive as to how an organisation must scope, build, document, or assess a system.

Implementation of the guidance provided by the Blueprint will differ depending on an organisation’s operating context and organisational culture. Organisations should implement the Blueprint in alignment with their existing change management, business processes and frameworks.

Placeholders such as `<ORGANISATION.GOV.AU>`, `<BLUEPRINT.GOV.AU>` and `<TENANT-NAME>` should be replaced with the relevant details as required.

{{% /alert %}}

### Name your policy

| Item        |                   Value |
| ----------- | ----------------------: |
| Name        | Safe attachments policy |
| Description |                  _None_ |

### Users and domains

| Item                                    |     Value |
| --------------------------------------- | --------: |
| Include these users, groups and domains |           |
| - Users                                 |    _None_ |
| - Groups                                |    _None_ |
| - Domains                               |    _None_ |
| Exclude these users, groups and domains | Unchecked |

### Settings

#### Safe Attachments unknown malware response

| Item                                      |                                                                            Value |
| ----------------------------------------- | -------------------------------------------------------------------------------: |
| Safe Attachments unknown malware response | Block - Block current and future messages and attachments with detected malware. |

#### Quarantine policy

| Item              |                 Value |
| ----------------- | --------------------: |
| Quarantine policy | AdminOnlyAccessPolicy |

#### Redirect messages with detected attachments

| Item            |     Value |
| --------------- | --------: |
| Enable redirect | Unchecked |

### Related information

#### Security and governance

- None identified

#### Design

- [Teams clients](/design/endpoints/applications/teams-clients)

#### Configuration

- None identified

#### References

- [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](https://learn.microsoft.com/en-au/defender-office-365/safe-attachments-for-spo-odfb-teams-configure)
