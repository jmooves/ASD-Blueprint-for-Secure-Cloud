---
title: "Rules"
weight: 015
description: "This section describes the configuration of endpoint rule settings within Microsoft Defender associated with systems built according to the guidance provided by ASD's Blueprint for Secure Cloud."
---

{{% alert title="Instruction" color="dark" %}}

The below tables outline the _as built_ configuration for ASD's _Blueprint for Secure Cloud_ (the Blueprint) for the Microsoft Defender portal at the following URL:

<https://security.microsoft.com/securitysettings/endpoints/alert_suppression>

The settings described on these pages provide a baseline implementation for a system configured using the Blueprint. Any implementation implied by these pages should not be considered as prescriptive as to how an organisation must scope, build, document, or assess a system.

Implementation of the guidance provided by the Blueprint will differ depending on an organisation’s operating context and organisational culture. Organisations should implement the Blueprint in alignment with their existing change management, business processes and frameworks.

Placeholders such as `<ORGANISATION.GOV.AU>`, `<BLUEPRINT.GOV.AU>` and `<TENANT-NAME>` should be replaced with the relevant details as required.

{{% /alert %}}

### Web Content Filtering

| Item                   |           Value |
| ---------------------- | --------------: |
| **General**            |                 |
| Policy Name            | Blocked content |
| **Blocked Categories** |                 |
| Adult content          |      Select all |
| High Bandwidth         |      Select all |
| Legal Liability        |      Select all |
| Leisure                |      Select all |
| Uncategorized          |      Select all |
| **Scope**              |                 |
| Machine Groups         |      Select all |

### Automation uploads

| Item                        |                                                                                                                                                      Value |
| --------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------: |
| **File Content Analysis**   |                                                                                                                                                            |
| Content analysis            |                                                                                                                                                         On |
| File extension names        | ",asp,aspx,bat,cmd,com,cpl,dll,docm,elf,exe,hta,img,inf,iso,jar,job,js,ko,ko.gz,lnk,msi,php,pl,pptm,ps1,py,rb,reg,scr,sh,so,sys,vb,vbe,vbs,vhd,ws,wsf,xlsm |
| **Memory Content Analysis** |                                                                                                                                                            |
| Enabled                     |                                                                                                                                                         On |

#### Security and governance

- None identified

#### Design

- [Endpoints and devices](/design/platform/security/endpoint-security)

#### Configuration

- [Configuration policies](/configuration/intune/devices/configuration-policies)
- [Endpoint security](/configuration/intune/endpoint-security)

#### References

- [Manage automation file uploads](https://learn.microsoft.com/en-au/defender-endpoint/manage-automation-file-uploads)
- [Web content filtering](https://learn.microsoft.com/en-au/defender-endpoint/web-content-filtering)
