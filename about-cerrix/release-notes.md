# Release Notes

On this page you’ll find a summary of new features, enhancements, bug fixes, and other changes included in each software update. This documentation is intended to keep you informed of the latest improvements and how they may impact your use of the platform.

For insight into our upcoming features and planned releases, please refer to our [Release Planning page](https://support.cerrix.com/portal/kb?btn=46\&id=54).

## May 2025

### **Budget-based risk management**

#### **Show budget in risks if budget-based risk scoring active**

In the risks, the budget is shown associated with the organization where the risk is defined for.

#### **Show financial impact in the workspace**

If the budget-based risk scoring is active, in the workspace the Gross and Net financial impact is shown per risk.

### **Incidents**

#### **Financial impact in workspace**

Total Gross and Net financial impact are shown in the workspace, for now in 1 column. Therefore, ordering and filtering is not yet possible. This will be further improved later.

#### **Sent mails overview**

As an administrator, all sent mails can be viewed via an extra tab in the incident module, in the Standing Data.

#### **Show Linked incidents in Risks and Controls**

If an incident is created and linked to a Risk or Control, that incident can also be found as a linked item in the specific Risk or Control. For Risks and Controls these incidents are shown in the existing page of linked events.

#### **Show Linked incidents for third parties affected**

If an incident was caused by a third party or the third party was affected, the incident can now be found as a linked incident. The incident link can also show the relation if the “+” sign is clicked. The details of date occurred, due date, description, and caused by, or affected by are shown.

#### **Date registered**

Date registered is now made available per incident in the workspace.

### **Notable Fixes**

#### **Control testplan import - Import of one-sample testplans**

The import of one-sample testplans resulted in testplans without a sample instead of testplans with one sample.

#### **Tasks - Extending tasks sometimes resulted in a task being created twice**

While extending a task, the previous end-date was included in the extension period. If a task is planned for that specific day, the task would be created again, resulting in a double task in the list.

#### **Customer Logo - The Logo format SVG caused problems in sending mails**

SVG Logo format is not accepted anymore by the system.

#### **Incidents - Notifications**

Notification email addresses for Incident types “Databreach” and “Operational incident” are not saved. Therefore, the mails to inform contact persons that a new incident of this type is created, were not sent. Now this has been fixed.

#### **Incidents - Required fields unclear warning**

If no “Responsible” or “Assessor” is assigned, the error was not clearly indicated in screen when saving the incident: under assigned, users can be added. Now the user can easily see what is missing.

#### **Incidents - MOI PowerBI**

PowerBI reports fail for MoIs of the type “Incident”. PowerBI will be improved to be able to handle Incident MoIs.

#### **Incidents - Deleted users**

Deleted Users used to be visible in the “Assigned Users” component. Now that has been fixed.

#### **Incidents - Missing values workspace**

The fields “Completed by” and “Closed on” were always empty columns in Incidents workspace.

#### **Incidents - Cannot delete Root cause**

Root cause in use in an incident could be deleted.

## April 2025

#### **New Incidents module**

We are introducing a new Incidents module which brings significant improvements over the current Events module, offering:

**Greater flexibility**

Easily create custom fields for each incident type, allowing full customization to match your organization’s needs.

**Streamlined workflows**

A single, standardized workflow for all incident types simplifies handling and tracking.

**Enhanced financial impact tracking**

Record financial impact per department and third party for improved reporting

**New and improved fields**

Includes a due date, support for Framework dimensions, and the ability to register third parties directly in incidents.

**Improved collaboration**

Discuss incidents directly within the incident page using built-in comments, enabling faster decision-making and follow-ups.

#### **Moving from Events to Incidents**

**Event Creation**

Once migrated, you will no longer be able to create new Events, but existing Events will remain viewable and editable.

**Form Updates**

Your existing forms used for Event creation will be automatically updated to create new Incidents.

**Standing Data**

All standing data from Events will be seamlessly transferred to Incidents.

## March 2025

#### **Third party**

**LEI code**

It is now possible to register the LEI code of a third party including a LEI code validity check. The LEI code is available in the workspace and API.

#### **Audit**

**Audit sponsor**

In an Audit, the Sponsor or Sponsors, can now be registered. The Sponsor could be, for instance, the initiator of the audit. The sponsor does not have any rights, not even view rights. In the document templates the field Sponsor(s) can be added.

#### **Risk**

**Budget-based risk scoring**

A new way of scoring risks has been made available. Budget-based risk scoring is the first set-up for this initiative. The purpose is to enable risk scoring based on an estimated financial impact in relation to an organizational budget.

This feature is still experimental. If you are interested, please submit a ticket in the Customer Portal.

{% content-ref url="../cerrix-functionalities/module-overview/risks/budget-based-risk-scoring.md" %}
[budget-based-risk-scoring.md](../cerrix-functionalities/module-overview/risks/budget-based-risk-scoring.md)
{% endcontent-ref %}

## February 2025

#### **Workspace preset hyperlink**

**Hyperlinks for public presets**

It is now possible in the Browse presets overview to create a link to a preset. If the preset is public, this link can be shared with other users via mail or messaging tool for instance. Please be aware that this is only possible for presets that are made public.

#### **Notable fixes**

**User management - Role group removal does not lead to removal of the associated roles for the user**

Role group removal did not lead to removal of the corresponding roles of the user. This issue has now been solved. After removing a role group for a user, the corresponding roles are removed for the user if no other active rolegroup for that user includes that role.

## January 2025

#### **Notable fixes**

**KRI - KRI restricted writer can't edit KRI datapoints**

KRI restricted writer could not edit KRI datapoints

**Audit - Unassigned Auditee cannot be requested to provide a document**

All users with the role Auditee could be asked via a mail request defined in the Audit to supply information to an audit. However, only users assigned to an Audit have the rights to do so. In this release both have been aligned: only Auditees assigned to the Audit can be asked to add information to an audit.\
