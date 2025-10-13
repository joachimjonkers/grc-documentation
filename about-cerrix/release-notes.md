# Release Notes

On this page you’ll find a summary of new features, enhancements, bug fixes, and other changes included in each software update. This documentation is intended to keep you informed of the latest improvements and how they may impact your use of the platform.

For insight into our release schedule for acceptance and production, please refer to our [Release Planning page](release-planning.md).

{% hint style="info" %}
The release notes are published shortly before a new release to the acceptance environment.
{% endhint %}

## ACC: 21 October 2025, PRD: 4 November 2025

#### Risk&#x20;

* **Custom fields**\
  Custom fields are now displayed in 2 columns and follow the order configured in the Standing data (In standing data the Administrator can configure settings for the application)

**Tasks**

* **API GET Update: identifier**\
  The Task "identifier" is now included in the Tasks API and Direct Data API for Tasks
* **API POST update: hyperlinks**\
  Hyperlinks can be included in the POST request for the Tasks API

{% hint style="info" %}
For more information about the Task API, click the question mark icon in the CERRIX application and go to "API Documentation".
{% endhint %}

**Incidents**

* **Standing data configuration**
  * It is now possible to change the name of the standard incident types "Data breach" and "Operational incident". &#x20;
  *   Move fields within a section and from 1 section to another

      It is now possible to reorganize the custom fields of an incident type by moving fields within a section and from 1 section to another. Note: Only the main tab "details" cannot be organized in this way
*   **Financial impact component ordering**

    Affected internal organizations and third parties are now shown below each other:&#x20;

    * On top all internal organizations are shown in the order that they are added,&#x20;
    * Below the organizations the third parties are shown in alphabetical order.  &#x20;
*   **Warning when removing incident type**

    A warning is shown if an incident type is removed and the associated tab contains data. The warning is introduced because these data in the incident type tab will be removed automatically.

### Notable Fixes&#x20;

#### **Risks**

* Restricted risk writers could create a risk for any internal organization\
  A user with only restricted rights can only view and edit risk of their own organizatio, Yet they were able to create a risk for any organization. This is now limited as well: restricted writers can only create a risk within their own organization.

#### **Forms**

* **Forms  freeze upon saving**\
  If a form contains multiple pages and the form is saved, the form "freezed" and could only be closed and reopened again to continue

**Incidents**

*   **System default preset update**

    System default preset was shown but it did not refresh the filter if clicked. The Default preset is not shown anymore, unless the preset is added as favorite.
*   **Assigned reporter**

    A reporter with no further rights should not be able to assign another reporter.&#x20;
*   **Preset preview**

    The Preset filter preview did not work anymore.

## ACC: 30 September 2025, PRD: 4 November 2025

#### General lay out

* **New CERRIX Logo.** \
  A new CERRIX logo is implemented in the application and in the mails sent via the application

**Tasks**

* **API Post: Update Task Score and Task Status**\
  A new API POST Update Task Score and Task Status. It is now possible to update the status and the score of Tasks via an API
* **Tasks Dataset**\
  A dataset of tasks is created. This data set can be used to create a Power BI overview for Tasks.

#### Incidents

* **Change the standard incident type tabs Operational Incident and Databreach**
  * To hide the standard fields defined in the associated tab. Please note that a field is hidden and is used in an Incident Form, the data entered in the Form for this field will still be mapped to the incident but it will not be visible because the field is hidden.
  * To add new sections and to add fields to all sections&#x20;
*   **Administrators can restore Deleted incidents**

    Deleted incidents are visible for the unrestricted Administrators as one of the categories of Deleted Items. Now it is possible to restore these deleted incidents as well.
*   **Incidents are included in Business assessments**&#x20;

    Incidents are now included in Business assessments: in the overviews generated via the Organizations & Business Dimensions Navigator.&#x20;

### Notable Fixes

#### **Data management**

* **Data management history details**\
  Details of History items could not be opened

**Business assessments**

* **Add documents as restricted process editor** \
  As restricted process editor it was not possible to add Assessment related document

**Incidents**

*   **Presets for Incident count widget**&#x20;

    If an incident preset is public (accessible for everyone) and used in a incident count widget on a CERRIX dashboard, it is not possible anymore to switch the preset to private, because that would break the count widget .

## ACC: 9 September 2025, PRD: 23 September 2025

#### Incidents

*   **Hyperlinks**

    At the location where documents can be added, it is now also possible to add hyperlinks. Hyperlinks can also be edited or deleted. Changes to hyperlinks can be tracked in the history.
*   **Administrators can view Deleted incidents**

    Deleted incidents are now visible for the unrestricted Administrators as one of the categories of Deleted Items. In a next sprint it will become possible to restore these deleted incidents.
*   **Comments section change of color of rejection comments**&#x20;

    Rejection messages in the comments section have a reddisch color to make them stand out from the rest of the messages.

#### **Tasks**

*   **Admin Permissions Update**&#x20;

    In tasks where no score is given yet, Administrators can now change task details and action dates without needing to add a score, even if it is a required field. This allows adjustments to task descriptions in response to changing circumstances.&#x20;
*   **Task Editing Enhancement**&#x20;

    Administrators can also edit fields such as Task Scoring, Comment, Documents, and Hyperlinks while a task is "in review," regardless of whether they are designated as a reviewer in the task configuration.

#### **API Update and Addition**

*   **Update of Direct data API "Task"**&#x20;

    The Task Status has been integrated into the direct data API "Task".
*   **New Post API for Tasks**

    A Post API is now available for adding tasks into CERRIX. This feature enables the execution of control tasks created outside of CERRIX within the CERRIX environment.

### Notable Fixes

#### BIM (MOI) export

*   **Visibility of selected MOIs report types**

    Resolved: If many reports are selected, the selection box did not show all these reports properly&#x20;

#### Business assessments

*   **Be able to end periodic reviews of Business Assessments**

    Now it is possible to end a periodic review in Business assessments, simply by changing the review frequency to "Single test". The next review date will be left empty and no error will appear.&#x20;

#### Forms

*   **File upload removal** &#x20;

    When deleting a "File upload" field from a Form with results linked to that field that still have a workflow unfinished, the application no longer throws an error.
*   **Unsaved changes pop-up**

    Form results that have un unfinished workflow status showed the "Unsaved changes pop-up even when no changes were made

#### Risk import

*   **Import with a risk with catalogue that has Event category as mandatory field**

    Resolved: A risk import sheet including a risk with risk catalogue with mandatory event category resulted in a validation error

## ACC: 19 August 2025, PRD: 23 September 2025

### Summary

Incident module gains richer history features, including document version tracking and custom field changes. The incident widget is improved and an incident count widget is introduced. Fixes include keeping personal incident presets private, form result handling, widget downloads, event linking, task scheduling, API stability, and MOI document updates.

### Incidents

* **Document history inside incidents**\
  A new **History** tab in the document information pop‑up lets users view current version details (uploader, timestamp, description, type) and browse/download prior versions. The list shows **User, Date, Type, Description, File size**, with improved filename hovers and consistent actions (“Edit document”, “Apply changes”).

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

* **Incident history now includes custom fields**\
  The incident history view now records **who changed what and when** for visible custom fields, grouped by incident type. Noise‑only records are hidden. Linked MOI history is excluded; financial impact changes show totals only.
* **Incidents count widget**\
  The **Module count widget** now supports the Incidents module, displaying the number of incidents as defined by a selected **public incident workspace preset**.
* **Incidents widget improvements**\
  Add a multiselect to **hide/show specific incident statuses** in the widget configuration (no filter by default). If an incident workspace tab is already open, clicking a data point now prompts to **load the new preset** before navigating.

#### Controls & Effectiveness Testing

* **Simpler view for non‑occurrence**\
  When a control **did not occur**, the source document area removes irrelevant sampling headers and shows either **“No source documents uploaded”** or only the uploaded source documents.

***

### Notable Fixes

#### Incidents

* **Email field validation no longer triggers too soon**\
  In incident type configuration, email validation now waits until users have **finished entering one or more addresses** (e.g., after separators), instead of triggering prematurely.
* **Correct tab icon highlighting**\
  The **Links**, **Attachments**, and **History** tab icons now highlight the **active** tab correctly when switching between them.
* **Personal incident presets stay private**\
  Newly created incident presets are **visible only to their creator** until explicitly set to **Public**; they no longer appear to other users by default.

#### Forms & Form APIs

* **Form results now include entered time**\
  Data breach form results now display **HH:MM** for time fields, and the workspace view shows the full **date & time** as expected.
* **Fetching results works after fields are deleted**\
  The **Get form results** API continues to return results even if fields/pages were removed after data collection; 404 errors are eliminated.

#### Dashboard & Widgets

* **Chart images download correctly**\
  Downloading a widget as an image (PNG/SVG) **no longer throws an error**.

#### Events

* **Custom field updates are saved**\
  Updating an event’s custom dropdown now **persists correctly**, with the value reflecting immediately after save.
* **Opening a linked event no longer errors (old Events module)**\
  When the **Incidents** setting is off, opening a linked event from risks/controls works without error in environments using the **older Events module**.

#### Tasks & Scheduling

* **Weekly repeat schedules stay correct after extending end date**\
  Weekly tasks that repeat (every 2/3/6 weeks) **retain the correct cadence** even after extending the schedule window.

#### Control Testing & Notifications

* **AcceptedReason now appears in acceptance emails**\
  The **\[AcceptedReason]** keyword correctly maps and displays the approver’s comment in acceptance notifications.
* **Correct API manual route for uploading source documents**\
  The Effectiveness Testing API documentation/route for **Upload Source Document (manual)** is corrected so calls reach the right endpoint.

#### APIs & Integrations

* **Finding Report API includes report name**\
  The DirectData **Finding Report API** now returns the **report name**, aligning the response with documentation and consumer expectations.
* **API key performance with large IP whitelists**\
  Requests using API keys with **very large IP whitelists** now execute efficiently without timeouts or excessive CPU usage.

#### MOI & Document Updates

* **Updating document type/description no longer fails in MOI**\
  Changing a MOI’s **document type** or **description** after upload no longer triggers a “mime type not specified” error.

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

For incidents the history of all standard items is made available via a third icon next to the icon for adding documents. <img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1).png" alt="" data-size="line">. The history shown is basic: only changes in the header and fields displayed in the details are now made available. History of linked items and custom fields will be included in a next release.

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

### AI Risk & Control Descriptions

The AI Risk & Control Descriptions Refinement functionalities are now available for all customers. Read more here: [ai-risk-description-refinement.md](../cerrix-functionalities/modules-overview/risks/ai-risk-description-refinement.md "mention"), [ai-control-description-refinement.md](../cerrix-functionalities/modules-overview/controls/ai-control-description-refinement.md "mention")

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

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Comment boxes can be enlarged via a pop-up

Sometimes a test comment requires more space than available in the control test screen. Pop-up signs have been added which, when clicked, the text is displayed in a large pop-up.

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Hover for attachment names

Attachments shown per test step were abbreviated if the name was longer than ca. 25 characters. To improve the readability, a hover is added so that the full name can easily be checked.

### Incidents

#### Warning is displayed when removing an incident type from an incident when data has already been entered in the incident type fields

A warning is displayed when clicking the "x" on an incident type for an incident type field that already contains data.

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

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
