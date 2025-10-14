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

## Risks Permission Matrix

<table><thead><tr><th width="245">Roles</th><th width="469">Description</th></tr></thead><tbody><tr><td>Risk Unrestricted Administrator</td><td>The Unrestricted Administrator has unrestricted read and write rights, can add entries in catalogues.</td></tr><tr><td>Risk Restricted Administrator</td><td>The Restricted Administrator has restricted read and write rights for his own organization.</td></tr><tr><td>Risk Unrestricted Writer</td><td>The Unrestricted Writer has write rights for the entire organization.</td></tr><tr><td>Risk Restricted Writer</td><td>The Restricted Writer has write rights for his own organization.</td></tr><tr><td>Risk Unrestricted Viewer</td><td>The Unrestricted Viewer has view rights for the entire organization.</td></tr><tr><td>Risk Restricted Viewer</td><td>The Restricted Viewer has read rights for his own organization.</td></tr></tbody></table>

You can see which permissions these roles have in this permission matrix:

{% file src="../.gitbook/assets/CERRIX-RISKS-PERMISSION-MATRIX-14-10-2025.xlsx" %}

