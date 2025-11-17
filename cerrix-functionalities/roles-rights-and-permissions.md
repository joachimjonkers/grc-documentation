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

## Controls Permission Matrix

<table><thead><tr><th width="239.72265625">Roles</th><th>Description</th></tr></thead><tbody><tr><td>Control Unrestricted Administrator</td><td>The Unrestricted Administrator is responsible for setting up and maintaining a complete overview of the Controls module across all organizations. This role grants full visibility and editing rights on all controls, as well as access to all standing data in the module. The user can also be assigned to any role within testing activities.</td></tr><tr><td>Control Restricted Administrator</td><td>The Restricted Administrator is also able to set up and keep the overview of the controls. However, the Restricted Administrator is limited to controls of his own organization. Also, the Restricted Administrator can be selected in every role in testing within his own organization.</td></tr><tr><td>Control Unrestricted Writer</td><td>The Unrestricted Writer has full write permissions for the Controls module across all organizations. They can create, edit, and delete controls but have no testing-related permissions.</td></tr><tr><td>Control Restricted Writer</td><td>The Restricted Writer can create, edit, and delete controls within their own organization. Similar to the Unrestricted Writer, this role does not include any testing rights.</td></tr><tr><td>Control Unrestricted Viewer</td><td>The Unrestricted Viewer can open and view all controls across all organizations in read-only mode. This role has no editing or testing permissions.</td></tr><tr><td>Control Restricted Viewer</td><td>The Restricted Viewer can open and view controls only within their own organization in read-only mode. This role has no editing or testing permissions.</td></tr><tr><td>Control Evidence Uploader</td><td>The Evidence Uploader can be assigned in test plans for both Design &#x26; Implementation and Effectiveness testing. This role is responsible for uploading and maintaining supporting evidence used during control testing.</td></tr><tr><td>Control Tester</td><td>The Tester is responsible for executing both Design &#x26; Implementation and Effectiveness testing. This role carries out control tests and documents the test results.</td></tr><tr><td>Control Reviewer</td><td>The Reviewer evaluates and approves the results of Effectiveness testing. This role is responsible for reviewing the tester’s work and ensuring that control assessments are complete and accurate.</td></tr><tr><td>Control Testplan Creator</td><td>The Test Plan Creator is responsible for designing and maintaining test plans for both Design &#x26; Implementation and Effectiveness testing. This role can also manage the corresponding test catalogues.</td></tr><tr><td>Control Executor</td><td>The Control Executor is responsible for performing the operational execution of controls as defined in the system. This role records the performance results and can upload relevant evidence demonstrating that the control has been executed according to plan.</td></tr></tbody></table>

You can see which permissions these roles have in this permission matrix:

{% file src="../.gitbook/assets/CERRIX-CONTROLS-PERMISSION-MATRIX-11-11-2025.xlsx" %}

## Controls Effectiveness Testing Permission Matrix

The role descriptions for Control Effectiveness Testing are the same as those for the [Controls](roles-rights-and-permissions.md#controls-permission-matrix).

You can see which permissions these roles have in this permission matrix:

{% file src="../.gitbook/assets/CERRIX-CONTROL EFFECTIVENESS TESTING-PERMISSION-MATRIX-17-11-2025.xlsx" %}
