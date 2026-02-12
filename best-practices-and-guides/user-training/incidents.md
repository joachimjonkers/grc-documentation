# Incidents

## Incidents

### Introduction

Incidents are events where something went wrong. In CERRIX, incident management helps you register, investigate, and learn from these events to prevent recurrence.

Unlike risks (which are things that might happen), incidents are things that have already happened. Proper incident management turns negative events into opportunities for improvement.

{% embed url="https://vimeo.com/1093634626" %}

#### Why Incident Management Matters

Without structured incident management:

* Events get reported but never investigated
* Root causes remain unknown and unaddressed
* Similar incidents keep occurring
* Lessons aren't learned or shared
* Compliance obligations aren't met

CERRIX incident management provides:

* **Structured registration** through Forms
* **Clear accountability** via role assignment
* **Investigation workflow** with status tracking
* **Root cause analysis** documentation
* **Preventive actions** through MoI linking
* **Complete audit trail** for compliance

#### How Incidents Connect to Other Modules

Incidents integrate with the entire CERRIX ecosystem:

* **Controls** – Incidents may indicate control failures
* **Risks** – Incidents prove that risks can materialize
* **MoIs** – Root cause analysis leads to preventive improvements
* **Testing** – Incident patterns inform testing priorities
* **Data Management** – Data breaches are a specific incident type

This integration ensures incidents drive continuous improvement rather than just generating reports.

#### Critical Requirement: Forms-Only Creation

> ⚠️ **IMPORTANT:** Incidents cannot be created directly in the Incidents workspace. They MUST be registered through Forms. This ensures consistent data collection and proper initial classification.

Your CERRIX administrator has configured incident registration Forms. These Forms capture all necessary information in a structured way and automatically create the incident in the system.

***

### Roles in Incidents

Incident management requires clear role definition to ensure accountability and thorough investigation.

#### Reporter

The Reporter is the person who witnesses or discovers the incident. They:

* Complete the incident registration Form
* Provide initial description and details
* May be contacted for clarification during investigation
* Should report promptly (while details are fresh)

**Anyone in the organization can be a Reporter.** Encouraging prompt reporting is essential for effective incident management.

#### Responsible

The Responsible party leads the investigation and resolution. They:

* Review the incident details
* Conduct or coordinate investigation activities
* Identify root causes
* Implement immediate containment actions
* Document findings and conclusions
* Create MoIs for preventive actions
* Update incident status through the workflow

**Choose someone with:** Authority in the affected area, investigation skills, resources to implement solutions

#### Delegate

The Delegate supports the Responsible party during investigation. They can:

* Gather evidence and documentation
* Interview witnesses
* Analyze technical details
* Draft investigation reports
* Upload supporting materials

**Important:** Delegates cannot change incident status. That responsibility remains with the Responsible party.

#### Reviewer / Auditor

The Reviewer or Auditor provides oversight and validation. They:

* Review investigation findings
* Verify root cause analysis is thorough
* Confirm corrective actions are appropriate
* Approve closure of the incident
* May require additional investigation if findings are insufficient

**Choose someone with:** Independence from the incident, senior perspective, quality assurance experience

***

### Incident Workflow

Understanding the incident workflow helps everyone know what's expected at each stage.

#### Status Progression

**1. Reported / Registered**

* Incident has been submitted through the Form
* Initial information is recorded
* Waiting for Responsible party assignment (if not assigned in Form)
* **Action needed:** Administrator or designated person assigns Responsible party

**2. Under Investigation**

* Responsible party has been assigned
* Investigation is being planned
* Evidence is being gathered
* Initial containment actions may be underway
* **Action needed:** Responsible party gathers facts, interviews witnesses, analyzes what happened

**3. In Progress**

* Root cause has been identified
* Corrective actions are being implemented
* MoIs may be created for systemic improvements
* Documentation is being completed
* **Action needed:** Responsible party implements fixes, documents findings, creates preventive MoIs

**4. Ready for Review**

* Investigation is complete
* All documentation is uploaded
* Corrective actions have been taken
* Waiting for validation
* **Action needed:** Reviewer assesses whether investigation is thorough and resolution is adequate

**5. Closed**

* Investigation approved by Reviewer/Auditor
* All actions completed
* Incident is now part of permanent record
* Data available for trend analysis
* **No further action needed**

{% embed url="https://vimeo.com/1093632244" %}

***

### Registering an Incident

> ⚠️ **CRITICAL REMINDER:** Most companies only create Incidents via Forms, not directly in the Incidents workspace to make it easier to register an Incident.

{% embed url="https://vimeo.com/1093634212" %}

#### How to Access the Form

Your organization has configured specific Forms for incident registration. The exact location depends on your CERRIX setup, but common access points include:

**Option 1: Direct Form Link**

* Your administrator provides a direct URL to the incident Form
* Bookmark this URL for easy access
* Share with colleagues who need to report incidents

**Option 2: Forms Menu**

* Navigate to the Forms section in CERRIX
* Select "Incident Registration" or similar
* Complete and submit

**Option 3: Quick Access Icon**

* Some organizations add an incident reporting icon to the main navigation
* Click to open the Form directly

> 💡 **Ask your CERRIX administrator** how your organization has configured incident Form access.

#### Completing the Form

**Basic Information**

**Incident name/title** – Give the incident a clear, descriptive title.

**Good examples:**

* "Customer payment data exposed via email error"
* "Fire suppression system activation in Server Room A"
* "Unauthorized access to HR shared drive"

**Weak examples:**

* "Incident 001"
* "Problem today"
* "Security thing"

**Incident type** – Select the category that best describes the incident.

**Incident date and time** – When did the incident occur? Be as precise as possible.

**Location/Department** – Where did the incident happen?

**Organisation** – Select the organization affected by the incident.

**Detailed Description**

**Incident description** – Describe what happened using the 5 W's + H:

* **What** happened?
* **When** did it happen?
* **Where** did it happen?
* **Who** was involved or affected?
* **Why** did it happen (if known)?
* **How** did it happen?

**Role Assignment**

**Responsible party** – Who will lead the investigation?

**Delegate** – Optional. Someone to assist with the investigation.

**Reviewer** – May be assigned later, or select now if clear.

**Evidence and Documentation**

Upload initial evidence: screenshots, photos, log files, or any relevant documentation.

#### Submitting the Form

After completing all sections, review your entries and click Submit.

***

### Investigating Incidents

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Incident Detail View - Main Tab]** Annotate:
>
> * "Incident details (type, date, description, impact)"
> * "Current status indicator"
> * "Responsible, Delegate, Reviewer fields"
> * "Tabs: Details, Comments, Documents, Event MoI, History"
> * "Status change dropdown"
> * "Save button"

Once assigned as Responsible, you'll guide the incident through investigation to resolution.

#### Investigation Steps

**1. Review Initial Information** – Read the incident description and evidence.

**2. Change Status to "Under Investigation"** – Signal that investigation has begun.

**3. Gather Additional Evidence** – Upload documents, logs, photos.

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Documents Tab]** Annotate:
>
> * "Documents tab selected"
> * "Upload document button"
> * "List of uploaded files with dates and uploaders"

**4. Document Progress** – Use the Comments tab to add investigation notes.

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Comments Tab]** Annotate:
>
> * "Comments tab selected"
> * "Add comment button"
> * "Comment history with timestamps and authors"

**5. Identify Root Cause** – Document your root cause analysis.

**6. Implement Corrective Actions** – Fix the immediate issue and document actions taken.

**7. Create MoIs for Prevention** – Navigate to the Event MoI tab and create improvement measures.

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Event MoI Tab]** Annotate:
>
> * "Event MoI tab selected"
> * "Add MoI button"
> * "List of linked MoIs (if any)"
> * "MoI details (name, status, responsible, due date)"

**8. Request Review** – Change status to "Ready for Review."

***

### Reviewing and Closing Incidents

#### As the Reviewer

When an incident reaches "Ready for Review," validate the investigation:

* Is root cause analysis thorough?
* Are corrective actions appropriate?
* Is evidence sufficient?
* Have appropriate MoIs been created?

If satisfactory, change status to "Closed." If insufficient, return to "In Progress" with feedback.

#### Tracking History

> 🖼️ **\[SCREENSHOT PLACEHOLDER: History Tab]** Annotate:
>
> * "History tab selected"
> * "Complete timeline of status changes"
> * "User actions (who did what when)"
> * "Comments added throughout process"
> * "Document uploads timeline"
> * "Complete audit trail"

The History tab provides complete audit trail for compliance and analysis.

***

### Best Practices

#### Reporting

* **Report promptly** – Don't delay while investigating
* **Focus on facts** – Describe objectively without blame
* **Be specific** – Provide details: dates, times, systems
* **Include evidence** – Capture it immediately

#### Investigating

* **Start immediately** – Evidence degrades over time
* **Be thorough but timely** – Set reasonable investigation timelines
* **Separate immediate and root causes** – Fix symptoms and systemic issues
* **Document as you go** – Don't wait until end

#### Prevention

* **Every incident yields learning** – Create MoIs to prevent recurrence
* **Target root causes** – Address why it happened, not just the incident itself
* **Link incidents to MoIs** – Create traceability

***

### Exercises

#### Exercise 1: Register an Incident

1. Access the incident registration Form
2. Complete all fields for a practice incident
3. Upload a sample document
4. Submit and find it in the workspace

#### Exercise 2: Investigate

1. Open your practice incident
2. Change status to "Under Investigation"
3. Add investigation comments
4. Upload evidence
5. Change status to "In Progress"

#### Exercise 3: Link an MoI

1. Navigate to Event MoI tab
2. Create an improvement measure
3. Link it to your incident
4. Change status to "Ready for Review"

#### Exercise 4: Review Audit Trail

1. Navigate to History tab
2. Review complete timeline
3. Note timestamps and actions
4. Understand compliance value

***

**Next Module:** Continue to **Finding Reports** to learn how to document audit results and link improvements to findings.
