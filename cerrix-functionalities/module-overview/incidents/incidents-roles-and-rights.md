# Incidents Roles & Rights

The Incidents module in CERRIX is built to support collaboration across multiple roles. Each role is designed with specific permissions to ensure the right level of access and responsibility for different users within your organization. Understanding these roles helps configure your incident management process effectively.

## Roles and Permissions

The Incidents module supports ten distinct user roles. Each role defines a set of permissions that grant access to specific parts of the module. Roles must be explicitly assigned to users. To provide broader access or responsibilities, users can be assigned multiple roles simultaneously.

<figure><img src="../../../.gitbook/assets/Screenshot 2025-07-04 165940.png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/Incidents Roles and rights3.png" alt=""><figcaption></figcaption></figure>

## Role Overview <a href="#toc530050983" id="toc530050983"></a>

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
