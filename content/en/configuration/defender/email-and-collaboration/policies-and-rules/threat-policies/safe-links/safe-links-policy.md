---
title: "Safe links policy"
weight: 005
description: "This section describes the configuration of the safe links policy settings within Microsoft Defender associated with systems built according to the guidance provided by ASD's Blueprint for Secure Cloud."
---

{{% alert title="Instruction" color="dark" %}}

The below pages outline the _as built_ configuration for ASD's _Blueprint for Secure Cloud_ (the Blueprint) for the Microsoft Defender portal at the following URL:

<https://security.microsoft.com/safelinksv2>

The settings described on these pages provide a baseline implementation for a system configured using the Blueprint. Any implementation implied by these pages should not be considered as prescriptive as to how an organisation must scope, build, document, or assess a system.

Implementation of the guidance provided by the Blueprint will differ depending on an organisation’s operating context and organisational culture. Organisations should implement the Blueprint in alignment with their existing change management, business processes and frameworks.

Placeholders such as `<ORGANISATION.GOV.AU>`, `<BLUEPRINT.GOV.AU>` and `<TENANT-NAME>` should be replaced with the relevant details as required.

{{% /alert %}}

### Name your policy

| Item        |             Value |
| ----------- | ----------------: |
| Name        | Safe links policy |
| Description |            _None_ |

### Users and domains

| Item                                    |     Value |
| --------------------------------------- | --------: |
| Include these users, groups and domains |           |
| - Users                                 |    _None_ |
| - Groups                                |    _None_ |
| - Domains                               |    _None_ |
| Exclude these users, groups and domains | Unchecked |

### URL & click protection settings

#### Email

| Item                                                                                                                   |     Value |
| ---------------------------------------------------------------------------------------------------------------------- | --------: |
| On: Safe Links checks a list of known, malicious links when users click links in email. URLs are rewritten by default. |   Checked |
| Apply Safe Links to email messages sent within the organization                                                        |   Checked |
| Apply real-time URL scanning for suspicious links and links that point to files                                        |   Checked |
| Wait for URL scanning to complete before delivering the message                                                        |   Checked |
| Do not rewrite URLs, do checks via Safe Links API only.                                                                | Unchecked |

#### Teams

| Item                                                                                                                      |   Value |
| ------------------------------------------------------------------------------------------------------------------------- | ------: |
| On: Safe Links checks a list of known, malicious links when users click links in Microsoft Teams. URLs are not rewritten. | Checked |

#### Office 365 Apps

| Item                                                                                                                            |   Value |
| ------------------------------------------------------------------------------------------------------------------------------- | ------: |
| On: Safe Links checks a list of known, malicious links when users click links in Microsoft Office apps. URLs are not rewritten. | Checked |

#### Click protection settings

| Item                                                                |     Value |
| ------------------------------------------------------------------- | --------: |
| Track user clicks                                                   |   Checked |
| Let users click through to the original URL                         | Unchecked |
| Display the organization branding on notification and warning pages |   Checked |

### Notification

| Item                              |    Value |
| --------------------------------- | -------: |
| Use the default notification text | Selected |

### Related information

#### Security and governance

- None identified

#### Design

- [Teams clients](/design/endpoints/applications/teams-clients)

#### Configuration

- None identified

#### References

- [Safe Links in Microsoft Defender for Office 365](https://learn.microsoft.com/en-au/defender-office-365/safe-links-about)
- [Set up Safe Links policies in Microsoft Defender for Office 365](https://learn.microsoft.com/en-au/defender-office-365/safe-links-policies-configure)
