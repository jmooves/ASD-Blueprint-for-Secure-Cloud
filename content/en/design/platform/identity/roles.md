---
title: Role-Based Access Control
weight: 20
description: "This section describes the design decisions associated with Role Based Access Control (RBAC) for system(s) built using ASD's Blueprint for Secure Cloud."
---

Role-Based Access Control (RBAC) defines what an end user or administrator can do. In relation to system administration, RBAC provides various roles each of which can only perform certain tasks. For example, help desk staff may be able to only view certain resources, whereas system administrators could view, create, and delete those resources.

Privileged Identity Management (PIM) can be leveraged to enhance the RBAC model available within Microsoft Entra ID. PIM is an implementation of Just-in-time (JIT) access, which ensures that an administrative account only has privileges when required to complete a function, and aligns to the principle of Zero Standing Privilege.

Each PIM role assignment can have the following attributes:

- **Activation Duration** - the Activation Duration attribute specifies the duration to allow the access request, the maximum is 24 hours.
- **Approver** - the Approver attribute specifies the person or people who can approve role activation requests.
- **Notification** - the Notification attribute specifies that a pending request is awaiting approval via email.
- **Incident Request Ticket** - the Incident Request Ticket attribute specifies that the approver add an incident ticket number to the approval request.
- **Multi-factor Authentication (MFA)** - the MFA attribute specifies whether MFA is required for activation.

Microsoft Entra ID roles can be assigned via PIM to various scope types, depending on the specific role being assigned. Scope types include:

- **Directory** - Roles that apply permissions across the entire Microsoft Entra ID tenant.
- **Administrative Unit** - Configurable by administrators to segregate permissions within organisation into specific business units or locations.
- **Application** - A specific application registered to Microsoft Entra ID.
- **Service Principal** - Including registered applications, managed identities and legacy apps.

{{% alert title="Note" color="info" %}}

Only [specific Microsoft Entra ID roles](https://learn.microsoft.com/entra/identity/role-based-access-control/admin-units-assign-roles#roles-that-can-be-assigned-with-administrative-unit-scope) can be assigned to the Administrative Unit scope type.

{{% /alert %}}

{{% alert title="Design decisions" color="warning" %}}

| Decision point             | Design decision                                                           | Justification                                                                                                                              |
| :------------------------- | :------------------------------------------------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------- |
| Role activation model      | Least Privilege via Privileged Identity Management                        | Enforces Just-in-Time access to reduce the attack surface of standing administrative privileges                                            |
| PIM role scope             | All Entra roles                                                           | Ensures consistent audit trails and access governance                                                                                      |
| Approval workflow          | Align approval requirements with the risk of each role’s capabilities     | Enforces dual control for high‑risk operations while enabling auto‑approval for routine, lower‑risk tasks to maintain operational velocity |
| Assignment type            | Eligible assignment                                                       | Prevents standing access by requiring active elevation for all in-scope administrative sessions                                            |
| Assignment duration        | Maximum 365 days                                                          | Enforces annual re-validation of administrative privileges in alignment with Essential Eight requirements                                  |
| Activation duration        | Capped at 8 hours and restricted to the minimum necessary duration        | Limits the exposure window of a compromised session while providing sufficient time for standard change windows                            |
| Standing access exceptions | Permanent active assignment for break glass and specific service accounts | Mitigates service replication delays and ensures emergency access availability during identity provider outages                            |

{{% /alert %}}

### Related information

#### Security and governance

- [Essential Eight - Restrict administrative privileges](/security-and-governance/essential-eight/restrict-administrative-privileges)

#### Design

- [Privileged Identity Management](/design/shared-services/microsoft-365/rbac/#privileged-identity-management)
- [Identity governance](/design/platform/identity/governance)
- [Role Based Access Control](/design/shared-services/microsoft-365/rbac)

#### Configuration

- None identified

#### References

- [Azure RBAC](https://learn.microsoft.com/entra/identity/role-based-access-control/custom-overview)
- [Entra ID Roles](https://learn.microsoft.com/entra/identity/role-based-access-control/permissions-reference)
- [Azure Resource Roles](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles)
- [Additional Microsoft 365 Roles](https://learn.microsoft.com/entra/identity/role-based-access-control/m365-workload-docs)
- [Entra ID Least privilege by Task](https://learn.microsoft.com/entra/identity/role-based-access-control/delegate-by-task)
- [Roles you can't manage in Privileged Identity Management](https://learn.microsoft.com/en-au/entra/id-governance/privileged-identity-management/pim-roles#what-about-microsoft-365-admin-roles)
