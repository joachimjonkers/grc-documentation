# Risks

## Risks

### Introduction

Risks form the foundation of risk management in CERRIX. They provide a structured way to capture events, their causes, and their effects within your organisation.

Controls mitigate these risks and help keep the organisation in control. Together with Testing and Measures of Improvement (MoIs), they form a complete cycle:

**Risk → Control → Testing → Improvement (MoI)**

This training explains how to create, link, and maintain risks in CERRIX.

> 📹 **\[VIDEO PLACEHOLDER: Risks Module Overview - 3 minutes]**
>
> * What risks are and why they matter
> * How risks connect to controls and testing
> * Real example of a risk in CERRIX

***

### Accessing the Risk workspace

Navigate to the Risk workspace from the main menu. This workspace gives you:

* A complete list of all risks at the detail level
* Central control over data quality
* The ability to create and save custom views with filters and sorting
* Export functionality to Excel or other formats

The Risk workspace is where you'll spend most of your time managing risk data. You can see all risks that belong to organisations you have access to, along with their current scores, owners, and linked controls.

***

### Creating a New Risk

> 📹 **\[VIDEO PLACEHOLDER: Creating Your First Risk ]**
>
> * Step-by-step walkthrough of creating a risk
> * Filling in all required fields
> * Understanding risk catalogue selection
> * Selecting dimensions and owners
> * Saving the risk

#### How to Get There

Open the Risk workspace and click **add new risk** in the top right corner.

#### Required Information

The "Create New Risk" form opens. Work through each section:

**Organisation** – Select the organisation responsible for this risk. This determines who has access to view and edit the risk.

**Risk catalogue** – Select the appropriate risk catalogue entry. Risk catalogues provide standardised risk definitions that ensure consistency across your organisation.

If subtypes are available in the dropdown, select the most specific option that matches your risk.

#### Risk Details

**Name** – Give the risk a concise name. In many cases, this will be pre-filled when you select a risk catalogue entry, but you can customise it as needed.

**Description** – Write a clear description that explains what the risk is. A good risk description follows the event-cause-effect structure:

* **Event:** What event could occur?
* **Cause:** What would cause this event?
* **Effect:** What would be the effect on the organisation?

**Cause** and **Effect** – These optional separate fields allow you to break down the cause and effect explicitly. Many organisations include this information directly in the risk description rather than using separate fields.

#### Dimensions and Categories

**Business dimensions** – Link the risk to specific processes, projects, or objectives. This makes it easier to generate targeted reports and understand which parts of your business are exposed to which risks.

Click the field and select from available business dimensions. You can select multiple dimensions.

**Framework dimensions** – Link to external frameworks like ISO 27001, DORA, or ISAE 3402. This is essential for compliance reporting.

**Risk Area** and **Event category** – These are typically populated automatically based on your risk catalogue selection. They provide additional categorisation for reporting purposes.

#### Ownership and Treatment

**Risk Owner** – Select the person who assesses and monitors this risk. Choose someone with direct knowledge of the risk area and the authority to make decisions about risk treatment.

**Risk treatment** – Indicate your intended approach to managing the risk:

* **Avoid** – Eliminate the activity that creates the risk
* **Transfer** – Move the risk to a third party (e.g., through insurance)
* **Reduce** – Implement controls to lower the likelihood or impact
* **Accept** – Acknowledge the risk and take no further action

#### Saving the Risk

Click **save** at the bottom of the form to create the risk.

The risk now appears in the Risk workspace and can be opened for scoring and linking to controls.

***

### Scoring Risks

#### Accessing Risk Scoring

After creating a risk (or opening an existing one), navigate to the **Risk scoring** tab to assess its severity.

#### Gross Risk Assessment

**Gross impact** and **gross likelihood** represent the risk before any controls are applied. This is your baseline assessment.

**Impact** measures the potential consequences if the risk materialises:

* Financial loss
* Reputational damage
* Regulatory penalties
* Operational disruption
* Data loss

**Likelihood** measures how probable the risk event is to occur within a given timeframe.

#### Net Risk Assessment

Once you've identified and implemented controls for this risk, you can assess the **net impact** and **net likelihood**. These scores reflect the reduced risk level after controls are working.

The difference between gross and net risk shows the effectiveness of your control environment. A large difference indicates strong control effectiveness.

#### Overall Risk Assessment

Use the **Overall risk assessment** field to indicate whether you accept the remaining (residual) risk or require further action.

This is particularly important for risks that remain high even after controls are applied.

#### Saving Risk Scores

Click **save** to record your risk scoring.

***

### Linking Controls to Risks

1. Click **Link panel** to open the control selection interface
2. Browse available controls or use search to find specific controls
3. Drag controls into the linked controls area, or click to select them
4. You can link multiple controls to a single risk

Choose controls that directly address the causes or reduce the impact of the risk. Not every control needs to be linked to every risk – focus on the controls that genuinely mitigate this specific risk.

> ⚠️ **Important:** Controls can only be linked if they belong to the same organisation as the risk. Cross-organisation linking is not supported.

#### Saving Control Links

When you've selected the appropriate controls, click **save** to establish the link.

#### Why Link Controls?

Linking controls to risks creates traceability in your GRC programme. It allows you to:

* See which risks are covered by which controls
* Identify gaps where risks lack adequate controls
* Generate reports showing the relationship between risks and controls
* Understand the impact when a control fails or needs changes
* Calculate net risk based on control effectiveness

***

### Best Practices

The quality of risk and control data in CERRIX determines how useful your analyses, reports, and audits will be. Follow these practices to ensure your information is clear, consistent, and actionable.

#### Use Event-Cause-Effect Structure

Every risk description should follow this structure so that everyone interprets the risk the same way:

* **Event:** What could happen?
* **Cause:** What would make it happen?
* **Effect:** What would the consequences be?

**Example:**

* **Event:** Unauthorised access to customer database
* **Cause:** Weak password policies and lack of multi-factor authentication
* **Effect:** Data breach resulting in regulatory fines, customer loss, and reputational damage

This structure ensures clarity and prevents misunderstandings.

#### Consistent Naming Conventions

Keep risk titles short and powerful, but ensure descriptions are complete. Follow the naming conventions agreed within your organisation.

**Good:** "Customer data breach via unauthorised access" **Weak:** "Security risk 1"

Consistency makes it easier to find risks, generate meaningful reports, and communicate with stakeholders.

#### Avoid Duplication

Before creating a new risk, check whether it already exists in the risk catalogue. Duplicate risks create noise in reports and make it difficult to understand your true risk profile.

Use the search and filter functions in the Risk workspace to check for existing similar risks.

#### Choose the Right Control Type

When you create controls, use the correct classification:

* **key control** – Critical for risk management, must be tested
* **requires monitoring** – Requires active oversight
* **Execution** – Describes how the control is performed (manual, automated)

This classification affects how controls appear in reports and testing programmes.

#### Link to Processes and Owners

Risks and controls only become truly useful when they're connected to processes, Business dimensions, and owners. These connections provide clarity and accountability across your organisation.

Always assign a Risk Owner and link to relevant Business dimensions.

#### Follow Frameworks and Conventions

Where possible, align with existing frameworks such as ISO, DORA, BIO, or internal standards. This makes audits simpler and reports more consistent with external requirements.

Use Framework dimensions to tag risks according to relevant standards.

***

### Exercises

#### Exercise 1: Create a New Risk

1. Open the Risk workspace
2. Click **add new risk**
3. Select your organisation
4. Choose a risk catalogue entry
5. Write a complete description using the event-cause-effect structure
6. Select Business dimensions
7. Assign a Risk Owner
8. Choose a Risk treatment approach
9. Click **save**

#### Exercise 2: Score the Risk

1. Open your newly created risk
2. Navigate to the **Risk scoring** tab
3. Assess and enter **gross impact** (1-5)
4. Assess and enter **gross likelihood** (1-5)
5. Note the gross risk score
6. If controls exist, enter **net impact** and **net likelihood**
7. Select an **Overall risk assessment**
8. Click **save**

#### Exercise 3: Link a Control

1. Stay in your risk detail view
2. Navigate to the **Linked controls** tab
3. Click **Link panel**
4. Search for or browse to find an appropriate control
5. Select the control (drag or click)
6. Click **save**
7. Verify the control appears in your Linked controls list

#### Exercise 4: Export Risks

1. Return to the Risk workspace
2. Apply a filter for a specific Framework dimension
3. Click **advanced configuration**
4. Set your filter criteria
5. Click **apply configuration**
6. Use the export function to download to Excel
7. Open the Excel file to verify the exported data

> 💡 **Practice Tip:** Complete all four exercises with the same risk to see the complete workflow from creation to linking and reporting.

***

**Next Module:** Now that you understand how to create and manage risks, continue to the **Controls** module to learn how to document the measures that mitigate these risks.
