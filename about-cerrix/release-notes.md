# Release Notes

On this page you’ll find a summary of new features, enhancements, bug fixes, and other changes included in each software update. This documentation is intended to keep you informed of the latest improvements and how they may impact your use of the platform.

For insight into our release schedule for acceptance and production, please refer to our [Release Planning page](release-planning.md).

{% hint style="info" %}
The release notes are published shortly before a new release to the acceptance environment.
{% endhint %}

## ACC: 29 July 2025, PRD: 12 August 2025

### Summary

* Tasks: Reviewers can now update task scores and edit the comments field.
* Incidents: Basic history is now available on the front page, and a new incident widget can be added to the dashboard.

### Tasks

Extended Reviewer Rights: For tasks with an assigned reviewer, the reviewer now has the ability to:

* Change the task score
* Edit the comments field
* Upload and attach documents

**Incident widget**

An incidents widget has been made available. The widget can be added to the dashboard. The incident widget shows the number of incidents in every status: waiting for acceptance, waiting for improvements, ready for review, rejected and approved.&#x20;

**Incident basic history**&#x20;

For incidents the history of all standard items is made available via a third icon next to the icon for adding documents. <img src="../.gitbook/assets/image (1).png" alt="" data-size="line">. The history shown is basic: only changes in the header and fields displayed in the details are now made available. History of linked items and custom fields will be included in a next release.

### General fixes

#### Count widget&#x20;

The count shown in the count widget was sometimes incorrect. It did not include all filtering in calculating the total. This was the case for Risks where always the unfiltered total of risks was shown and for other count widgets the organization filter was not included in the count.

**Incidents**&#x20;

It is not possible anymore to create an incident without a name&#x20;

In dropdowns filter values kept on being displayed and could be confused with actual values. This issue is solved

## ACC: 15 July 2025, PRD: 12 August 2025

### Summary

A new API for Forms is added. In the incident module sections are made visible and foldable, and fixes for exports and financial impact visibility.&#x20;

### Forms

#### API-driven form entries

With this API Forms results can be created.  So forms can be populated through data gathered by other applications. Limitations: All field names of the Form are unique. It is not possible to use these form results for creating new incidents (via “mapbacking”). More information can be found in the API documentation (see the “?”  in the top right of the CERRIX APP)

### Incidents Module

#### Page sections

Sections defined for an incident type are made visible in the incident type tabs. Sections are shown with a title. The first section is always called “Details”. This Details section is only visible if more sections are defined.

&#x20;

### General fixes

#### Forms workflow review comments

Form workflow review comments were not completely shown. Issue is resolved.

#### &#x20;API Module

Help icons in API key settings

The help icons in the API key settings don't redirect to the relevant API documentation page. This will be fixed in our next release.

#### Controls Module

Controls workspace column “Latest period score”

The column “Latest period score” in the Controls workspace now correctly displays the latest period score, instead of the first period score.

&#x20;Incidents Module

#### Exports

Fixed the issue that Exports could fail because of old data formats.

#### Financial impact

The financial impact component was not fully visible for lower resolution screens. As solution for these situations a scroll bar appears.

#### Financial impact in workspace

The workspace column “Financial impact Gross & Net” now will display values in correct format in all cases and the export will contain these values as well.

## ACC: 24 June 2025, PRD: 8 July 2025

## Summary

This release includes updates across several core modules including Incidents, Control Testing, Roles & Permissions, AI Assistant, Test Plans, and KRI Management. Below is a categorized summary of improvements and fixes.

### **Incidents Module**

#### **Uniform Menu Text Color**

All left-side menu items now use a consistent white text color, improving readability and eliminating display inconsistencies between sections.

#### **Linked Items Icon Update**

The icon for linked items has been modernized to enhance visual clarity and align with CERRIX’s updated design language.

#### **Document Versioning Support**

Users can now replace incident documents with new versions directly in the interface. The updated design includes:

* A "Drop file or browse to replace" option.
* Uploader details (username + timestamp) displayed below the filename.
* Streamlined access controls (edit rights required).

The complete history will be made available in a later release

### **Measures of Improvement**

#### **Display Incident Details in MOI Workspace**

Incident details (identifier, name, description) are now consistently displayed in the MOI workspace for incident-based MOIs. This aligns with how other MOI types are presented, ensuring a unified user experience.

### **Control Testing**

#### **Enhanced Email Notifications for Control Testing**

Period names and test plan details are now included in control testing emails and notifications. For notifications, periods appear in the "Controls" table (empty for simple testing).

#### **Expanded Control Effectiveness Catalogue**

Added default fields to streamline test plan creation:

* **New section**: Sample generation (method + manual reason).
* **Default Test Information**: Source/evidence/test instructions.
* **Default Involved Persons**: Review settings (reviewer + yes/no toggle).\
  Sections renamed for clarity (e.g., "Method of testing" → "Default Test Steps").

### **Risk Module**

#### **Optional Likelihood Validation**

A new environment setting allows net likelihood to exceed gross likelihood for risks (disabled by default). When enabled, the system skips validation checks during imports or saves.

### Navigation

#### **Help Menu Redesign**

The help menu has been reorganized for clarity, with new links and icons:

* **Product Documentation**: External link to [docs.cerrix.com](https://docs.cerrix.com/).
* **API Documentation**: Internal link to the API documentation.
* **Release Notes**: External link to release notes.
* **Support**: External link to support resources.
* **About CERRIX**: Unchanged.

***

### Notable Fixes

**Incidents Module**

**Startup Cache Issues**

Resolved crashes causing application downtime by fixing cache-loading logic during startup, particularly affecting incident-module URL fetching.

**Default Incident Type Options**

Added default dropdown options for "Operational Incident" and "Databreach" in case no drop-down options are defined yet, for example during environment setup, to prevent save/export errors.

**Deleted User Role Consistency**

Fixed inconsistent behavior where deleting a user removed them from the "Reporter" role in incidents. All roles (Assessor, Responsible, Informed, Reporter) now retain deleted users (deleted users are marked with `*`).

**General Fixes**

#### **KRI Writer Edit Permissions**

KRI restricted writers can now edit KRI datapoints. Previously, changes were not saved.

#### **Role Group Wizard**

* **Role Removal**: Roles are now correctly removed from users when deleted via the wizard.
* **User Removal**: Users are no longer retained in role groups after removal via the wizard.

#### **AI-Generated Risk Descriptions**

Fixed formatting issues where line breaks in AI responses incorrectly split risk descriptions into multiple suggestions.

#### **Test Plan Mandatory Fields**

"Sample Generation Method" is now properly validated as mandatory during test plan creation using the "copy from catalogue" option. UI indicators (red outline/❌ icon) alert users if left empty.

### Known issues

#### Help icons in API key settings

The help icons in the API key settings don't redirect to the relevant API documentation page. This will be fixed in our next release.



## ACC: 3 June 2025, PRD: 8 July 2025

### Control testing improvements

#### Show historical control details

In control tests, the control details are shown in a dropdown field on the right side. The ID, Name, but also frequency, execution method, and description are available.

Because the testing done at the time of the actual testing is based on the control description that was valid at that time, the historic values are shown: the name, description, frequency and execution method as they were defined at that time of the control test.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Comment boxes can be enlarged via a pop-up

Sometimes a test comment requires more space than available in the control test screen. Pop-up signs have been added which, when clicked, the text is displayed in a large pop-up.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Hover for attachment names

Attachments shown per test step were abbreviated if the name was longer than ca. 25 characters. To improve the readability, a hover is added so that the full name can easily be checked.

### Incidents

#### Warning is displayed when removing an incident type from an incident when data has already been entered in the incident type fields

A warning is displayed when clicking the "x" on an incident type for an incident type field that already contains data.

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Ability to add files when creating an incident via a Form

Files included in a Form result which is used to create an incident, are now included in that incident.

#### All users that add an incident will be registered as incident reporter

All users, even users without the role “Reporter”, who add an incident via a Form, will be registered as incident reporters.

#### Incident types can be archived

Archiving an incident type results in users not being able to create an incident of this type anymore. In the workspace these fields belonging to the archived incident were hidden. Incidents that already have this incident type will show the archived incident type.

An incident administrator can archive an incident type via the standing data tab “Configuration”.

### Notable fixes

#### Periodic MOIs - Users that have no role in the workflow of an MOI should not receive notifications

Users who are removed from an MOI still get a periodic notification about the MOI. This has been fixed.

#### Documents -  Document information

In MOIs and Audit, for instance, the information about a document was not fully available, and the description was not visible. This has been fixed.

#### Incidents

#### **Financial impact in workspace**

The financial impact for Gross and Net amounts were displayed as JSON (code), instead of numbers. With this change both variables are now displayed as numbers. They are still shown together in one column. This will be improved later to enable searching and ordering the workspace based on these numbers.

#### Notification email addresses for standard Incident types Databreach and Operational incident are not saved

In Standing Data, in tab Configuration, you can specify which Email addresses receive a message whenever an incident of that type is created. However, saving these addresses for the default types “Databreach” and “Operational incident” was not possible. That has been fixed.

#### Predefined incident type names like “Databreach” and “Operational incident” looked editable

Predefined incident type names looked editable, but they are not. So now it is not possible to edit the names.

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

As an administrator, all sent mails can be viewed via an extra tab in the incident module, underneath the Standing Data.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (2) (1) (1).png" alt=""><figcaption></figcaption></figure>

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
