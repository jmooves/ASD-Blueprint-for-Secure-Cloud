---
title: "Quarantine policy"
weight: 005
description: "This section describes the configuration of quarantine policy settings within Microsoft Defender associated with systems built according to the guidance provided by ASD's Blueprint for Secure Cloud."
---

{{% alert title="Instruction" color="dark" %}}

The below pages outline the _as built_ configuration for ASD's _Blueprint for Secure Cloud_ (the Blueprint) for the Microsoft Defender portal at the following URL:

<https://security.microsoft.com/safelinksv2>

The settings described on these pages provide a baseline implementation for a system configured using the Blueprint. Any implementation implied by these pages should not be considered as prescriptive as to how an organisation must scope, build, document, or assess a system.

Implementation of the guidance provided by the Blueprint will differ depending on an organisation’s operating context and organisational culture. Organisations should implement the Blueprint in alignment with their existing change management, business processes and frameworks.

Placeholders such as `<ORGANISATION.GOV.AU>`, `<BLUEPRINT.GOV.AU>` and `<TENANT-NAME>` should be replaced with the relevant details as required.

{{% /alert %}}

### Policy name

| Item        |             Value |
| ----------- | ----------------: |
| Policy name | Quarantine policy |

### Recipient message access

| Item                                                                  |                                                                Value |
| --------------------------------------------------------------------- | -------------------------------------------------------------------: |
| Recipient message access                                              |                                       Set specific access (Advanced) |
| Select release action preference                                      | Allow recipients to request a message to be released from quarantine |
| Select additional actions recipients can take on quarantined messages |                                                                      |
| - Delete                                                              |                                                              Checked |
| - Preview                                                             |                                                              Checked |
| - Block sender                                                        |                                                              Checked |
| - Allow sender                                                        |                                                            Unchecked |

### Quarantine notification

| Item                                                                |    Value |
| ------------------------------------------------------------------- | -------: |
| Enable                                                              |  Checked |
| - Don't include quarantined messages from blocked sender addresses. | Selected |

### Related information

#### Security and governance

- None identified

#### Design

- [Teams clients](/design/endpoints/applications/teams-clients)

#### Configuration

- [Microsoft Teams Protection](/configuration/defender/system/settings/email-and-collaboration/microsoft-teams-protection)

#### References

- [Quarantine policies in cloud organizations](https://learn.microsoft.com/en-au/defender-office-365/quarantine-policies)
