# Controls

## Controls

### Introduction

Controls (also called beheersmaatregelen) mitigate risks within your organisation. A control can be preventive, detective, or repressive.

Together with risks and testing, controls form the foundation of your GRC process. They demonstrate that your organisation is actively managing its risks and maintaining control.

This training explains how to:

* Create controls in CERRIX
* Link controls to risks
* Work with control attributes and execution frequency
* Ensure controls are properly classified and documented

***

### Accessing the Controls Workspace

Navigate to the Controls Workspace from the main menu. The workspace provides:

* A complete list of all controls at the detail level
* Central oversight of control quality and coverage
* The ability to create and save custom views with filters and sorting
* Export functionality to Excel or other formats

The Controls Workspace shows all controls belonging to organisations you have access to, along with their types, frequencies, owners, and linked risks.

***

### Creating a New Control

> 📹 **\[VIDEO PLACEHOLDER: Creating Your First Control - 8 minutes]**
>
> * Complete walkthrough of creating a control
> * Using the 5W 1H model for descriptions
> * Setting control attributes correctly
> * Linking to dimensions and frameworks

#### How to Get There

Open the Controls Workspace and click **add new control** in the top right corner.

#### Control Catalogue

The "Create New Control" form opens. Start with these required fields:

**Control catalogue** – Select the appropriate category in the control catalogue. Like risk catalogues, control catalogues provide standardised control definitions. If subtypes are available, select the most specific option.

**Organisation** – Select the organisation responsible for this control. This determines access rights and which risks can be linked to the control.

#### Naming and Description

**Name** – Give the control a clear and descriptive name that makes its purpose immediately obvious.

**Description** – Write a comprehensive description of the control. We recommend using the **5W 1H model**:

> 💡 **Tip:** Use the [AI functionality in Controls](https://docs.cerrix.com/cerrix-functionalities/module-overview/controls/ai-control-description-refinement) for guidelines on the Control Description&#x20;

**Example:** "**Who:** IT Security Manager **What:** Reviews all active user accounts and access permissions against current employee list **Where:** IT Department **With what:** Active Directory, HR system employee export **When:** Monthly, first Monday of each month **What if:** Unauthorised access detected → immediate account suspension and incident report"

A complete description using this structure eliminates ambiguity and ensures everyone understands exactly what the control entails.

#### Control Classification

**key control** – Tick this box if the control is critical to your risk management. Key controls must be tested and monitored more rigorously.

> 💡 **Tip:** Not every control is a key control. Reserve this designation for controls that are essential to managing your most significant risks.

**requires monitoring** – Select this if the control needs active monitoring and periodic testing. Not all controls require formal monitoring – use this designation thoughtfully.

**in place** – Tick this if the control is already implemented and operating. Leave unchecked for controls that are still being designed or rolled out.

#### Linking Dimensions

**Business dimensions** – Connect the control to specific processes or projects. This improves traceability and helps generate targeted reports.

Click the field and select from available business dimensions. You can select multiple.

**Framework dimensions** – Link the control to external standards such as ISAE 3402, ISO 27001, or DORA. This is essential for audit and compliance reporting.

#### Saving the Control

Click **save** to create the control.

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Save Button Location]**

The control now appears in the Controls Workspace and can be opened to add detailed attributes.

***

### Additional Control Details

> 📹 **\[VIDEO PLACEHOLDER: Control Attributes and Properties - 5 minutes]**
>
> * Setting control type (preventive, detective, repressive)
> * Configuring execution method and frequency
> * Assigning control owners
> * Understanding RACI roles

After creating the basic control, you can add more detailed attributes that describe how it operates.

#### Opening Your Control

1. Find your control in the Controls Workspace
2. Click on the control row to open the detail view
3. The main information tab opens by default

#### Internal Classification

**Aspect internal** – Categorise the control according to your organisation's internal control framework. This might align with frameworks like COSO or your organisation's specific risk taxonomy.

**Type** – Select whether the control is:

* **detective** – Identifies issues after they occur
* **preventive** – Stops issues from occurring
* **repressive** – Corrects issues that have occurred

> 💡 **Understanding Control Types:**
>
> * **Preventive:** Password complexity rules, segregation of duties, approval workflows
> * **Detective:** Log reviews, reconciliations, monitoring alerts
> * **Repressive:** Incident response procedures, backup restoration, remediation actions

Most controls are either detective or preventive. Understanding the control type helps you assess whether your control environment is balanced.

#### Ownership

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Owner Field]**

**Owner** – Designate who is responsible for the control. This person ensures the control is executed correctly and addresses any issues that arise.

Choose someone with direct operational knowledge of the control and the authority to make changes when needed.

#### Execution Method

**Control execution** – Indicate how the control is performed:

* **Manual** – Human-performed activities
* **Automated** – System-enforced controls
* **Semi-automated** – Combination of system and human activities

Automated controls are generally more reliable but less flexible. Manual controls require more oversight but can adapt to exceptions.

#### Execution Frequency

**Control frequency** – Record how often the control is executed:

* Continuous (automated controls)
* Daily
* Weekly
* Monthly
* Quarterly
* Annually
* Ad hoc (event-driven)

> ⚠️ **Important:** Be realistic when setting frequency. Overstating frequency creates unrealistic testing expectations. Understating it may expose your organisation to unnecessary risk.

#### Optional Information

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Optional Fields Section]** Annotate:
>
> * "RACI field"
> * "Cost field"
> * "Comments field"

You can also record:

* **RACI** – Who is Responsible, Accountable, Consulted, and Informed
* **Cost** – The financial or resource cost of operating the control
* **Comments** – Any additional context or special circumstances

#### Saving Additional Details

Click **save** to record these details.

***

### Linking Risks to Controls

Controls exist to mitigate risks. Linking them together creates a complete picture of how your organisation manages risk.

#### Adding Risks

1. Click **Link panel** to open the risk selection interface
2. Browse available risks or use search
3. Drag risks into the linked risks area, or click to select
4. You can link multiple risks to a single control

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Link Panel for Risks]** Annotate:
>
> * "Available risks"
> * "Search/filter"
> * "Drag-and-drop or click to select"

> 💡 **Tip:** Link only the risks that this control genuinely mitigates. Over-linking creates false confidence and makes it harder to identify genuine control gaps.

#### Saving Risk Links

When you've selected the appropriate risks, click **save**.

***

### Best Practices

Controls are the backbone of risk management in CERRIX. Poorly described or incorrectly classified controls lead to:

* Confusion among colleagues
* Incomplete or inaccurate reports
* Problems during audits or testing

Follow these practices to ensure your controls are consistent, clear, and complete.

#### Be Concrete and Complete

Use the **5W 1H** structure when writing control descriptions:

* **Who** performs the control?
* **What** actions are taken?
* **Where** is it performed?
* **With what** tools or systems?
* **When** is it executed?
* **What if** something goes wrong?

A complete description eliminates ambiguity and ensures the control can be tested effectively.

#### Apply Classification Correctly

* **Key control** = Critical to risk management, must be tested
* **Requires monitoring** = Needs active oversight and periodic testing
* **Execution method** = Manual, automated, or semi-automated

Correct classification determines how the control appears in reports and testing schedules.

#### Set Realistic Frequency

Don't inflate control frequency unnecessarily. If a control is performed monthly, record it as monthly – not weekly. Unrealistic frequencies create impossible testing burdens.

At the same time, don't understate frequency if the control genuinely runs more often. The frequency should reflect reality.

#### Assign Clear Ownership

Every control must have a designated owner – a person or department responsible for its execution. Without clear ownership, controls become neglected and ineffective.

#### Always Link to Risks

A control that isn't linked to any risk has no clear purpose. Link controls to the risks they mitigate to create traceability and demonstrate the value of your control environment.

#### Use Business and Framework Dimensions

These connections make controls more useful in dashboards and external reports. Framework dimensions are particularly important for audit and compliance purposes (e.g., ISAE 3402, DORA, BIO).

***

### Exercises

#### Exercise 1: Create a New Control

1. Open the Controls Workspace
2. Click **add new control**
3. Select a control catalogue entry
4. Select your organisation
5. Write a complete description using the **5W 1H** convention:
   * **Who:** Who executes the control?
   * **What:** What is done during execution?
   * **Where:** Where is the control performed?
   * **With what:** What systems or documents?
   * **When:** How often (frequency)?
   * **What if:** What if the control fails?
6. Select Business dimensions
7. Select Framework dimensions
8. Tick **in place** if the control is operational
9. Click **save**

#### Exercise 2: Add Control Attributes

1. Open your newly created control
2. Set **aspect internal** (if applicable)
3. Select **type** (detective, preventive, or repressive)
4. Assign an **owner**
5. Set **control execution** method (manual, automated, semi-automated)
6. Set **control frequency** (daily, weekly, monthly, etc.)
7. Add optional information (RACI, cost, comments) if desired
8. Click **save**

#### Exercise 3: Link Risks

1. Stay in your control detail view
2. Navigate to the **Linked risks** tab
3. Click **Link panel**
4. Search for or browse to find appropriate risks
5. Select risks that this control mitigates
6. Click **save**
7. Verify the risks appear in your Linked risks list

#### Exercise 4: Export Controls

1. Return to the Controls Workspace
2. Apply a filter for a specific Framework dimension
3. Click **advanced configuration**
4. Set your filter criteria
5. Click **apply configuration**
6. Use the export function to download to Excel
7. Open the Excel file to verify the exported data

***

**Next Module:** Now that you understand how to create and manage controls, continue to the **Control Testing** module to learn how to prove these controls are effective in practice.
