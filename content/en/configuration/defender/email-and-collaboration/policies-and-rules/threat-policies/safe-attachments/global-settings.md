---
title: "Global settings"
weight: 005
description: "This section describes the configuration of safe attachments global settings within Microsoft Defender associated with systems built according to the guidance provided by ASD's Blueprint for Secure Cloud."
---

{{% alert title="Instruction" color="dark" %}}

The below pages outline the _as built_ configuration for ASD's _Blueprint for Secure Cloud_ (the Blueprint) for the Microsoft Defender portal at the following URL:

<https://security.microsoft.com/safelinksv2>

The settings described on these pages provide a baseline implementation for a system configured using the Blueprint. Any implementation implied by these pages should not be considered as prescriptive as to how an organisation must scope, build, document, or assess a system.

Implementation of the guidance provided by the Blueprint will differ depending on an organisation’s operating context and organisational culture. Organisations should implement the Blueprint in alignment with their existing change management, business processes and frameworks.

Placeholders such as `<ORGANISATION.GOV.AU>`, `<BLUEPRINT.GOV.AU>` and `<TENANT-NAME>` should be replaced with the relevant details as required.

{{% /alert %}}

### Global settings

| Item                                                                                                 |    Value |
| ---------------------------------------------------------------------------------------------------- | -------: |
| Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams                        |  Enabled |
| Turn on Safe Documents for Office clients.                                                           |  Enabled |
| Allow people to click through Protected View even if Safe Documents identified the file as malicious | Disabled |

### Related information

#### Security and governance

- None identified

#### Design

- [Safe attachments](/design/shared-services/defender/safe-attachments)
- [Teams clients](/design/endpoints/applications/teams-clients)

#### Configuration

- None identified

#### References

- [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](https://learn.microsoft.com/en-au/defender-office-365/safe-attachments-for-spo-odfb-teams-configure)
