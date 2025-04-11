# Incidents Workflow

The **Incidents module** in CERRIX is designed to streamline the process of handling incidents within your organization, providing a structured and auditable workflow. This guide walks you through the **standard flow** of an incident's lifecycle and highlights key actions and interface elements you can interact with during the process.

***

## Overview of the Incident Workflow

The **Incident Workflow** guides users through each required step in processing incidents, clearly showing the current status and future actions needed.

At the top of the incident screen, you'll see a clear visualization of the workflow steps:

* Completed steps are **highlighted green**.
* Available next steps are clearly indicated, showing what actions can currently be performed.
* Future steps are visible but inactive until prior required steps have been completed.

> **Note:** Only assigned users can perform actions at each workflow step.

<figure><img src="../../../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

***

## Key Steps in the Workflow

### **Incident Creation**

Read more about creating a new incident in this article:

{% content-ref url="creating-a-new-incident.md" %}
[creating-a-new-incident.md](creating-a-new-incident.md)
{% endcontent-ref %}

***

### Assessing & Evaluating an Incident

After an incident has been reported:

1. To continue with processing, select either:
   * **Accept incident** to move forward.
   * **Reject incident** if it's invalid or incorrect.
   * Leave a comment (required). This comment will be visible in the [#chat-and-incident-history](incidents-workflow.md#chat-and-incident-history "mention")
2. Click **Confirm**.
   * The **"Assessing"** workflow status at the top of the page changes to **green**, indicating the incident is officially confirmed.
   * The incident now moves to the **Improving** stage.

<figure><img src="../../../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

***

### **Linking Related Items**

In the **Assessing, Improving or Review** stage, you’ll see a **Link** icon![](<../../../.gitbook/assets/image (28).png>)which can be used to link relevant items by clicking on the linking button:

* **Link existing Risks or Controls**
  * Use the dedicated button to select relevant items from the system.
* **Create a Measure of Improvement (MOI)**
  * Opens a new tab for MOI creation.

<figure><img src="../../../.gitbook/assets/image (26).png" alt=""><figcaption></figcaption></figure>

***

### Business and Framework Dimensions

Additional configuration dimensions include:

* **Business Dimensions** Allow associating incidents with particular business dimensions defined in your system.
* **Framework Dimensions** Facilitate linking incidents to your organization's compliance and internal control frameworks.

<figure><img src="../../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

***

### **Attach Supporting Documents**

* Click on the **Attach** icon ![](<../../../.gitbook/assets/image (30).png>)
* Drag and drop or select a file to upload.
* Files will be attached directly to the incident for context and traceability.

<figure><img src="../../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

***

### Review and Closing an Incident

At the **Review** stage, the incident has the status **Ready for Review**:

1. Review all linked data, documents, and details carefully.
2. When satisfied, click **Approve & close**, or click **Reject**:
   * The incident workflow finishes, and the incident moves to a **read-only** state.
   * The workflow view clearly indicates that the incident is completed and can no longer be edited.

***

### **Final Decision: Approve or Reject**

* From the **"Ready to Review"** status:
  * **Approve and Close** to complete the incident lifecycle.
  * Once closed, the incident gets the status **Completed** and becomes **read-only**.

***

## Chat and Incident History

The incident page includes an interactive **Chat and History Pane** accessible from the right side:

* View complete audit trails of incident updates, statuses, notes, and decisions made throughout the workflow.
* Use this pane for update notes. Future releases will enable direct chat functionalities among incident participants for additional collaboration.

<figure><img src="../../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

***

## Workflow Notifications

Notifications automatically alert relevant users when the incident advances through workflow stages:

* Notification behaviors in the **Incidents** module mirror those in the existing **Events** module used within your CERRIX environment.
* In your production environment, relevant stakeholders will receive notifications upon workflow status changes (e.g., confirmation, review readiness, approval).
* In this demonstration environment, notifications are inactive, but in production, known standard processes apply.

> **Note:** If your existing CERRIX configuration refers to these as "Events," you might consider standardizing your terminology to "Incidents" for clarity, though this naming choice remains flexible.
