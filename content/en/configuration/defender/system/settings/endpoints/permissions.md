---
title: "Permissions"
weight: 010
description: "This section describes the configuration of endpoint permissions settings within Microsoft Defender associated with systems built according to the guidance provided by ASD's Blueprint for Secure Cloud."
---

{{% alert title="Instruction" color="dark" %}}

The below tables outline the _as built_ configuration for ASD's _Blueprint for Secure Cloud_ (the Blueprint) for the Microsoft Defender portal at the following URL:

<https://security.microsoft.com/securitysettings/endpoints/user_roles>

The settings described on these pages provide a baseline implementation for a system configured using the Blueprint. Any implementation implied by these pages should not be considered as prescriptive as to how an organisation must scope, build, document, or assess a system.

Implementation of the guidance provided by the Blueprint will differ depending on an organisation’s operating context and organisational culture. Organisations should implement the Blueprint in alignment with their existing change management, business processes and frameworks.

Placeholders such as `<ORGANISATION.GOV.AU>`, `<BLUEPRINT.GOV.AU>` and `<TENANT-NAME>` should be replaced with the relevant details as required.

{{% /alert %}}

### Roles

#### Microsoft Defender for Endpoint Administrator (default)

| Item                     |                                          Value |
| ------------------------ | ---------------------------------------------: |
| **General**              |                                                |
| _All settings_           |                        _Modification disabled_ |
| **Assigned user groups** |                                                |
| Group Name               | `<Defender for Endpoint administration group>` |

#### Microsoft Defender for Endpoint Remediation

| Item                                                                              |                                       Value |
| --------------------------------------------------------------------------------- | ------------------------------------------: |
| **General**                                                                       |                                             |
| Role name                                                                         | Microsoft Defender for Endpoint Remediation |
| Description                                                                       |                                      _None_ |
| View Data                                                                         |                                     Checked |
| - Security operations                                                             |                                     Checked |
| - Defender Vulnerability Management                                               |                                     Checked |
| Active remediation actions                                                        |                                     Checked |
| - Security Operations                                                             |                                     Checked |
| - Defender Vulnerability Management - Exception handling                          |                                     Checked |
| - Defender Vulnerability Management - Remediation handling                        |                                     Checked |
| - Defender Vulnerability Management - Application handling                        |                                     Checked |
| Defender Vulnerability Management - Manage security baselines assessment profiles |                                     Checked |
| Alerts investigation                                                              |                                     Checked |
| Manage security settings in Security Center                                       |                                   Unchecked |
| Live response capabilities                                                        |                                     Checked |
| - Advanced                                                                        |                                    Selected |
| **Assigned User groups**                                                          |                                             |
| Group Name                                                                        | `<Defender for Endpoint remediation group>` |

#### Microsoft Defender for Endpoint Viewer

| Item                                                                              |                                  Value |
| --------------------------------------------------------------------------------- | -------------------------------------: |
| **General**                                                                       |                                        |
| Role name                                                                         | Microsoft Defender for Endpoint Viewer |
| Description                                                                       |                                 _None_ |
| View Data                                                                         |                                Checked |
| - Security operations                                                             |                                Checked |
| - Defender Vulnerability Management                                               |                                Checked |
| Active remediation actions                                                        |                              Unchecked |
| - Security Operations                                                             |                              Unchecked |
| - Defender Vulnerability Management - Exception handling                          |                              Unchecked |
| - Defender Vulnerability Management - Remediation handling                        |                              Unchecked |
| - Defender Vulnerability Management - Application handling                        |                              Unchecked |
| Defender Vulnerability Management - Manage security baselines assessment profiles |                              Unchecked |
| Alerts investigation                                                              |                              Unchecked |
| Manage security settings in Security Center                                       |                              Unchecked |
| Live response capabilities                                                        |                              Unchecked |
| **Assigned User groups**                                                          |                                        |
| Group Name                                                                        |   `<Defender for Endpoint view group>` |

### Device groups

#### Windows 10/11

| Item              |                           Value |
| ----------------- | ------------------------------: |
| Rank              |                               1 |
| **General**       |                                 |
| Device group name |                   Windows 10/11 |
| Remediation level |                Full remediation |
| Description       |                          _None_ |
| **Devices**       |                                 |
| Name              |                _Not configured_ |
| AND Domain        |                _Not configured_ |
| AND Tag           |                _Not configured_ |
| AND OS            |     In - Windows 11, Windows 10 |
| **User access**   |                                 |
| Group Name        | `<Device administration group>` |

#### Ungrouped devices

| Item              |                                                             Value |
| ----------------- | ----------------------------------------------------------------: |
| Rank              | _Not applicable for the ungrouped devices (default) device group_ |
| **General**       |                                                                   |
| Device group name |                                       Ungrouped devices (default) |
| Remediation level |                                                  Full remediation |
| **Devices**       |           _Not applicable for the default ungrouped device group_ |
| **User access**   |                                                                   |
| Group Name        |                                   `<Device administration group>` |

### Related information

#### Security and governance

- [System management](/security-and-governance/system-security-plan/system-management)

#### Design

- [Endpoints and devices](/design/platform/security/endpoint-security)

#### Configuration

- None identified

#### References

- [Create and manage device groups](https://learn.microsoft.com/en-au/defender-endpoint/machine-groups)
- [Create and manage roles for role-based access control](https://learn.microsoft.com/en-au/defender-endpoint/user-roles)
