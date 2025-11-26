---
title: "User reported settings"
weight: 005
description: "This section describes the configuration of user reporting settings within Microsoft Defender associated with systems built according to the guidance provided by ASD's Blueprint for Secure Cloud."
---

{{% alert title="Instruction" color="dark" %}}

The below tables outline the _as built_ configuration for ASD's _Blueprint for Secure Cloud_ (the Blueprint) for the Microsoft Defender portal at the following URL:

<https://security.microsoft.com/securitysettings/userSubmission>

The settings described on these pages provide a baseline implementation for a system configured using the Blueprint. Any implementation implied by these pages should not be considered as prescriptive as to how an organisation must scope, build, document, or assess a system.

Implementation of the guidance provided by the Blueprint will differ depending on an organisation’s operating context and organisational culture. Organisations should implement the Blueprint in alignment with their existing change management, business processes and frameworks.

Placeholders such as `<ORGANISATION.GOV.AU>`, `<BLUEPRINT.GOV.AU>` and `<TENANT-NAME>` should be replaced with the relevant details as required.

{{% /alert %}}

#### Outlook

| Item                                                   |    Value |
| ------------------------------------------------------ | -------: |
| Monitor reported messages in Outlook                   |  Checked |
| Use the built-in Report button in Outlook              | Selected |
| - Ask the user to confirm before reporting             |  Checked |
| - Show a success message after the message is reported |  Checked |

#### Microsoft Teams

| Item                                         |   Value |
| -------------------------------------------- | ------: |
| Monitor reported messages in Microsoft Teams | Checked |

#### Reported message destinations

| Item                                                         |                                     Value |
| ------------------------------------------------------------ | ----------------------------------------: |
| Send reported messages to:                                   |        Microsoft and my reporting mailbox |
| Add an exchange online mailbox to send reported messages to: | `<REPORTING-MAILBOX@ORGANISATION.GOV.AU>` |

#### Email notifications

| Item                                                                                                                             |     Value |
| -------------------------------------------------------------------------------------------------------------------------------- | --------: |
| Automatically email users the results of the investigation. Includes results for reported messages from all monitored platforms. | Unchecked |
| Specify a Microsoft 365 mailbox to use as the From address of email notifications                                                | Unchecked |
| Replace the Microsoft logo with my organization's logo across all reporting experiences.                                         |   Checked |

#### Reporting from quarantine

| Item                                                                                         |   Value |
| -------------------------------------------------------------------------------------------- | ------: |
| Allow reporting for quarantined messages. Only admins can report quarantined Teams messages. | Checked |

### Related information

#### Security and governance

- None identified

#### Design

- [Teams clients](/design/endpoints/applications/teams-clients)

#### Configuration

- [Messaging](/configuration/teams/setting-and-policies/global-settings/messaging/messaging)

#### References

- [User reported message settings in Microsoft Teams](https://learn.microsoft.com/en-au/defender-office-365/submissions-teams)
- [User reported settings](https://learn.microsoft.com/en-au/defender-office-365/submissions-user-reported-messages-custom-mailbox)
