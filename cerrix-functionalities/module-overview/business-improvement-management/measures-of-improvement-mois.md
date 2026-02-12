# Measures of Improvement (MoI's)

{% hint style="info" %}
**Video Tutorial**

Prefer to watch instead of read? Have a look at our [#measures-of-improvement-mois](../../../best-practices-and-guides/video-tutorials.md#measures-of-improvement-mois "mention") Video Tutorials
{% endhint %}

<figure><img src="../../../.gitbook/assets/MOI Workflow v2.jpg" alt=""><figcaption></figcaption></figure>

The MOIs module is designed to address recurring issues or ineffective controls by implementing corrective measures. This module ensures that improvements are executed and reviewed effectively.

### Introduction

Measures of Improvement (MoIs) are CERRIX's way of turning problems into solutions. When testing reveals control weaknesses, when incidents occur, or when audits find issues, MoIs ensure these findings lead to concrete improvements rather than just reports.

MoIs provide structured tracking from identification through resolution, with clear accountability and complete audit trails.

#### Why MoIs Matter

Without structured improvement tracking, findings and issues get documented but never resolved. MoIs prevent this by:

* Creating accountability through role assignment
* Enforcing deadlines and progress tracking
* Providing visibility into improvement programmes
* Generating audit evidence of corrective actions
* Closing the loop from problem identification to solution implementation

#### How MoIs Connect to Other Modules

MoIs can be created from:

* **Risks** – When risk assessment identifies needed improvements
* **Controls** – When control design needs enhancement
* **Test Plans** – When effectiveness testing reveals control failures
* **Incidents** – When root cause analysis identifies preventive actions
* **Finding Reports** – When audits require corrective actions

This integration means problems identified anywhere in CERRIX automatically flow into structured improvement tracking.

***

### Roles in Improvement Management

Every MoI has clearly defined roles, each with specific responsibilities in the improvement process.

#### Responsible

The Responsible party owns the improvement action. This person:

* Plans and executes the improvement
* Updates progress and status
* Uploads evidence of completion
* Moves the MoI from "In progress" to "Ready for acceptance"
* Ensures the action meets its deadline

**Choose someone with:** Direct operational authority, necessary resources, relevant expertise

#### Delegate

The Delegate assists the Responsible party. They can:

* Execute specific tasks assigned to them
* Upload supporting documentation
* Add comments and updates
* Work on the improvement alongside the Responsible party

**Important:** Delegates cannot change the MoI status or close it. Final accountability remains with the Responsible party.

#### Reviewer

The Reviewer validates that improvements are properly implemented. They:

* Review evidence provided by the Responsible party
* Verify improvements meet the original requirement
* Approve actions by marking them "Accepted"
* Reject insufficient actions, returning them to "In progress"
* Ensure quality before the MoI can be closed

**Choose someone with:** Independence from execution, technical knowledge to assess quality, authority to require rework

#### Auditor

The Auditor provides oversight of the entire improvement process. They typically:

* Create MoIs based on audit findings or test failures
* Monitor progress across multiple improvements
* Close MoIs after Reviewer approval
* Maintain the audit trail
* Report on improvement programme effectiveness

**Note:** Not all MoIs require an Auditor. This role is most common for audit-driven improvements.

***

### Creating a New MoI

{% embed url="https://vimeo.com/1015659974/dc9b044570" %}

#### Where to Create MoIs

MoIs can be created from multiple locations. The most common are:

**From a Risk:**

1. Open the risk
2. Navigate to the **Risk MoI** tab
3. Click **Add MoI**

**From a Control:**

1. Open the control
2. Navigate to the **Control Improvement MoI** tab
3. Click **Add MoI**

**From a Test Plan:**

1. Open the test plan
2. Navigate to the **Control Improvement MoI** tab
3. Click **Add MoI**

**From an Incident:**

1. Open the incident
2. Navigate to the **Event MoI** tab
3. Click **Add MoI**

**From a Finding Report:**

1. Open the finding report
2. Navigate to the **Linked Measures of Improvement** tab
3. Click **Add MoI**

The create form is the same regardless of where you start, but the source link is automatically established.

#### Steps for Creating

When the Create MoI form opens, work through these sections:

**Core Information**

**Name** – Give the MoI a clear, action-oriented name that describes what will be improved.

**Subject** – Select the category that best describes this improvement (e.g., Access Control, Data Protection, Testing Process).

**Priority** – Assess urgency:

* **High** – Critical issues, regulatory requirements, significant risks
* **Medium** – Important improvements, moderate impact
* **Low** – Nice-to-have enhancements, minor issues

**Implementation score** – Rate current implementation on a 1-5 scale:

* **1** – Not implemented at all
* **2** – Partially defined, not operational
* **3** – Implemented but inconsistent
* **4** – Largely implemented and working
* **5** – Fully implemented and effective

> 💡 **Tip:** The implementation score helps track progress. Update it as work proceeds to show improvement.

**Planning**

**Start date** – When work will begin. This helps with resource planning and timeline reporting.

**Due date** – Deadline for completion. Be realistic but appropriately urgent. Consider:

* Regulatory deadlines
* Risk severity
* Resource availability
* Dependency on other work

**Role Assignment**

**Responsible** – The person who will execute this improvement. They must have the authority and resources to implement the action.

**Delegate** – Optional. Someone who will assist the Responsible party. Useful for large improvements requiring multiple people.

**Reviewer** – Who will validate that the improvement is properly implemented. Choose someone with appropriate technical knowledge and independence.

**Auditor** – Optional. Often used when the MoI comes from an audit finding. The auditor provides oversight and closes the MoI after approval.

> ⚠️ **Important:** Don't assign the same person as both Responsible and Reviewer. This creates a conflict of interest and weakens quality control.

**Details**

**Finding description** – Describe the issue or gap that needs improvement. Be specific about what's wrong and why it matters.

**Example:** "Current password policy allows passwords as short as 6 characters with no complexity requirements. This creates vulnerability to brute-force attacks and doesn't meet ISO 27001 requirements."

**Recommendation** – Specify exactly what should be done to address the finding.

**Example:** "Update password policy to require minimum 12 characters with complexity requirements (uppercase, lowercase, number, special character). Implement system enforcement and user communication."

**Management response** – Document management's position on the finding and proposed action.

**Example:** "Management agrees with the recommendation and will implement the updated password policy by end of Q2. IT Security will lead implementation with support from Communications team for user notification."

**Comments** – Any additional context, dependencies, or considerations.

**Linking**

**Business dimensions** – Connect the MoI to relevant processes, departments, or projects. This enables targeted reporting.

**Linked risks** – Connect to risks that will be reduced by this improvement.

**Linked controls** – Connect to controls that will be strengthened by this improvement.

**Documents** – Attach supporting evidence, analysis, or reference materials.

These links create traceability showing why the improvement matters and what it affects.

#### Saving the MoI

After completing all sections, click **save**.

The MoI is now created and visible in the MoI workspace. The Responsible party will receive notification of their assignment.

***

### MoI Workflow

{% embed url="https://vimeo.com/1047426213/2c823a7fa9" %}

Understanding the MoI workflow helps you know what to do at each stage and what happens next.

#### Status Progression

**1. Unconfirmed**

* MoI has been created
* Assigned to Responsible party
* Waiting for Responsible party to confirm they'll execute it
* **Action needed:** Responsible party reviews and accepts the assignment

**2. In progress**

* Responsible party has accepted the assignment
* Work is underway
* Evidence is being gathered
* **Action needed:** Responsible party executes the improvement, uploads evidence, updates progress

**3. Ready for acceptance**

* Responsible party has completed the work
* Evidence has been uploaded
* Waiting for Reviewer validation
* **Action needed:** Reviewer assesses quality and evidence

**4. Accepted / Rejected**

* **Accepted:** Reviewer confirms the improvement is satisfactory
* **Rejected:** Reviewer finds the improvement insufficient
* **Action needed (if rejected):** Responsible party addresses feedback and resubmits

**5. Closed**

* Improvement is complete and verified
* Auditor (or system) has closed the MoI
* Action is now part of permanent audit trail
* **No further action needed**

#### Status Transitions

Only certain roles can change status:

* **Responsible → Auditor/System:** Unconfirmed → In progress
* **Responsible:** In progress → Ready for acceptance
* **Reviewer:** Ready for acceptance → Accepted or Rejected
* **Reviewer:** Rejected → In progress
* **Auditor:** Accepted → Closed

These restrictions ensure proper oversight and prevent improvements from being prematurely closed.

***

### Working with MoIs

#### As the Responsible Party

When you're assigned as Responsible:

1. **Review the assignment** – Understand what's required, by when, and what success looks like
2. **Confirm acceptance** – Change status from "Unconfirmed" to "In progress"
3. **Execute the improvement** – Do the work specified in the recommendation
4. **Document progress** – Add comments and upload evidence as you go
5. **Submit for review** – When complete, change status to "Ready for acceptance"

#### As the Reviewer

When an MoI reaches "Ready for acceptance":

1. **Review the evidence** – Check uploaded documents and completion notes
2. **Verify implementation** – Confirm the improvement actually addresses the original finding
3. **Make a decision:**
   * **Accept** if the improvement is satisfactory → Status becomes "Accepted"
   * **Reject** if more work is needed → Status returns to "In progress" with feedback

#### As the Auditor

When an MoI is "Accepted":

1. **Perform final verification** – Ensure all requirements are met
2. **Review audit trail** – Check that proper process was followed
3. **Close the MoI** – Change status to "Closed"

#### Tracking History

The History tab shows:

* All status changes
* Who made each change and when
* Comments added throughout the process
* Document uploads
* Reviewer feedback

This complete audit trail demonstrates due diligence and supports compliance evidence.

***

### Best Practices

#### Creating Effective MoIs

**Be specific in descriptions** – Vague findings lead to vague improvements. "Improve security" is useless. "Implement MFA for all privileged accounts by Q2" is actionable.

**Use SMART criteria:**

* **Specific** – Exactly what will be improved
* **Measurable** – How you'll know it's done
* **Achievable** – Realistic given resources
* **Relevant** – Actually addresses the finding
* **Time-bound** – Clear deadline

**Link to source** – Always connect MoIs to the risk, incident, or finding that triggered them. This creates traceability.

**Add evidence early and often** – Don't wait until completion. Upload documents as you progress to show ongoing work.

#### Setting Realistic Deadlines

**Consider complexity** – Simple process changes might take weeks. System implementations might take months.

**Account for dependencies** – If you need budget approval, vendor procurement, or training development, factor those timelines in.

**Include buffer** – Unexpected delays happen. Build in contingency time.

**Respect regulatory deadlines** – If a regulator requires remediation by a specific date, work backward from that deadline.

#### Providing Good Feedback

When rejecting an MoI, be constructive:

**Bad:** "Not good enough, redo it."

**Good:** "The password policy document has been updated, but system enforcement isn't implemented yet. Please work with IT to configure Active Directory to enforce the new requirements, then resubmit with evidence of enforcement."

Specific feedback helps the Responsible party understand exactly what's needed.

#### Closing the Loop

After closing an MoI:

* Update the related risk score to reflect reduced risk
* Update control effectiveness ratings
* Document lessons learned for future improvements
* Consider whether testing is needed to verify sustained implementation

MoIs aren't complete until the improvement is embedded in operations and verified through testing.

***

### Reporting and Analysis

#### Using MoI Data

The MoI workspace and reporting features let you analyze your improvement programme:

**Status overview** – How many MoIs are open, in progress, or overdue?

**Responsible party workload** – Who has the most assigned improvements?

**Priority distribution** – Are we focusing on high-priority issues?

**Time to completion** – How long does it typically take to close MoIs?

**Rejection rate** – What percentage of MoIs require rework?

These metrics help you:

* Identify bottlenecks in the improvement process
* Allocate resources effectively
* Improve time-to-resolution
* Demonstrate improvement programme effectiveness to stakeholders

#### Common Reports

**Overdue MoIs** – Critical for management attention

**High Priority Open Items** – Shows most urgent work

**MoIs by Source** – Understand which risks/incidents/findings generate most improvements

**Completion Rate Trends** – Are we getting better at closing improvements?

***

### Exercises

#### Exercise 1: Create an MoI

1. Navigate to the Risk workspace
2. Open any risk that lacks adequate controls
3. Click on the **Risk MoI** tab
4. Click **Add MoI**
5. Complete all required fields:
   * Name: "Implement quarterly vendor security assessments"
   * Priority: High
   * Responsible: Assign to yourself
   * Reviewer: Assign to a colleague
   * Due date: 90 days from now
   * Finding description: Describe the gap
   * Recommendation: Specify the improvement
6. Link to Business dimensions
7. Click **save**

#### Exercise 2: Progress Through Workflow

Using the MoI you created:

1. Open the MoI from the MoI workspace
2. Change status from "Unconfirmed" to "In progress"
3. Add a comment describing your implementation plan
4. Upload a sample document as evidence (any document for practice)
5. Update the implementation score to show progress
6. Change status to "Ready for acceptance"
7. (If practicing with a colleague) Have them review and provide feedback
8. Review the History tab to see your audit trail

#### Exercise 3: Review MoI Reporting

1. Return to the MoI workspace
2. Apply a filter to show only "In progress" MoIs
3. Sort by due date to identify approaching deadlines
4. Create a preset called "My Active MoIs" showing items where you're Responsible
5. Export the filtered list to Excel
6. Review the exported data to understand available fields
