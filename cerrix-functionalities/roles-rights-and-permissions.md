# Roles, Rights and Permissions

CERRIX uses a role-based access model to manage who can view, edit, and approve information across the platform. This ensures that every user only has access to the functions and data they need for their responsibilities, supporting both data security and efficient collaboration.

## Roles and Permissions in CERRIX

Each user is assigned one or more roles, which define their level of access. Roles are aligned with common responsibilities in governance, risk, compliance, audit, and incident management. Permissions specify what a role can do within a module.&#x20;

## Permission Matrices per Module

CERRIX provides a Permission Matrix for each key module. These matrices are the authoritative reference for configuring and validating user rights. In the matrix sheet:

* Each row lists a specific action (e.g., _Can report new incidents_, _Can delete risks_).
* Each column represents a role (e.g., Risk Unrestricted Admin, Incident Assessor).
* The cells indicate whether the role has permission, and what the scope of their permission is (_Unrestricted_, _Restricted_, or _Assigned_).
  * Unrestricted means that a user has rights across all organizations
  * Restricted means that a user has rights for a specific organization

## Incidents Permission Matrix

The Incidents module in CERRIX is built to support collaboration across multiple roles. Each role is designed with specific permissions to ensure the right level of access and responsibility for different users within your organization. Understanding these roles helps configure your incident management process effectively.

### Roles and Permissions

The Incidents module supports eight distinct user roles. Each role defines a set of permissions that grant access to specific parts of the module. Roles must be explicitly assigned to users. To provide broader access or responsibilities, users can be assigned multiple roles simultaneously.

| Role                             | Description                                                                                                                              |
| -------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- |
| Event Unrestricted Administrator | Full access to all event-related functionality and visibility across all organizations.                                                  |
| Event Restricted Administrator   | Similar to the Unrestricted Administrator but limited to their own organization (and daughters org) and without access to Standing data. |
| Event Assessor                   | Full editing rights (in statuses: Awaiting acceptance and Ready for review) for events assigned to them                                  |
| Event Responsible                | Editing rights (in status Awaiting improvements) for assigned events, except for user assignments.                                       |
| Event Reporter                   | Can report new events for any organization in CERRIX.                                                                                    |
| Event Informed                   | View-only access to events where the user is assigned.                                                                                   |
| Event Unrestricted Viewer        | View-only access to all events, across all organizations.                                                                                |
| Event Restricted Viewer          | View-only access to events within the user’s own organization (and daughters org)                                                        |

You can see which permissions these roles have in this permission matrix:

{% file src="../.gitbook/assets/CERRIX-INCIDENT-PERMISSION-MATRIX-17-09-2025.xlsx" %}
