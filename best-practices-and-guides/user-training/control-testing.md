# Control Testing

## Control Testing

### Introduction

Control Testing is the process that determines whether controls are well-designed, properly implemented, and working effectively in practice. In CERRIX, this process consists of three interconnected components:

1. **Design & Implementation (D\&I) Testing**
2. **Control Execution**
3. **Effectiveness Testing**

#### Why Control Testing Matters

Control testing provides evidence that risks are genuinely under control. It creates confidence among internal and external stakeholders, including auditors and regulators. Testing makes it visible whether controls are working consistently and where improvements are needed. The results feed directly into reports and improvement measures (MoIs).

#### Who Is Involved?

* **Control Owners** – Execute controls and register evidence (Control Execution)
* **Testers** – Assess control quality through D\&I and Effectiveness Testing
* **Reviewers** – Evaluate test results produced by testers
* **Auditors** – Use test results for internal and external assurance

Each role has distinct responsibilities that together ensure comprehensive control assurance.

***

### Control Testing Framework in CERRIX

#### Design & Implementation (D\&I) Testing

D\&I Testing assesses whether the control is well-designed and correctly configured.

This includes evaluation of:

* Documentation and written procedures
* System configurations and technical settings
* Integration with business processes
* Alignment with the control's intended purpose

**Example:** An authorisation process is documented in procedures and technically configured in an access management system. D\&I testing verifies that both the documentation and system settings are correct and aligned.

#### Control Execution

Control Execution is the actual performance of the control by the owner or responsible department.

This involves:

* Performing the control activities as documented
* Registering execution in CERRIX (e.g., uploading checklists, updating status, attaching evidence)
* Creating an audit trail for later testing

Execution is the foundation for effectiveness testing – without documented execution, there's nothing to test.

#### Effectiveness Testing

Effectiveness Testing determines whether the control works in practice as intended.

This includes:

* Sample-based testing of actual control executions
* Review of supporting evidence and documentation
* Assessment of whether the control achieved its objective

**Example:** Sample testing demonstrates that user authorisations were correctly applied in practice, not just configured in theory.

***

### Design & Implementation Testing

#### Creating a D\&I Test Plan

D\&I testing typically happens once when a control is first implemented or when significant changes are made to the control design.

**How to Get There**

1. Open the **Controls Workspace**
2. Select the control you want to test
3. Click on the **Effectiveness testing** tab
4. You'll see an overview of all test plans and test periods for this control

> 💡 **Note:** Both D\&I Testing and Effectiveness Testing are managed from the same "Effectiveness testing" tab within a control. The tab provides a unified view of all testing activities for that control.

**Managing Test Periods**

Click **Manage test periods** to define the timeframe for testing:

1. Enter the period (e.g., Q1 2026, FY 2026)
2. Specify the number of samples to be tested
3. Click **save**

Test periods provide structure for your testing programme and help organise evidence collection.

**Adding a Test Plan**

Click **Add test plan** to create a new D\&I test. The test plan wizard opens automatically and guides you through:

**1. Assigning roles:**

* **Tester** – Who will perform the testing
* **Evidence uploader** – Who provides supporting documentation
* **Reviewer** – Who validates the test results

**2. Defining scope:**

* Which control is being tested
* Which period is covered
* What aspects of design and implementation will be evaluated

**3. Setting parameters:**

* Sample sizes (if applicable)
* Specific testing criteria
* Expected evidence types

Click **save** to finalise the test plan.

**Workflow Activation**

After saving the test plan, tasks are automatically placed in the calendars of all involved parties. This ensures everyone knows their responsibilities and deadlines.

Examples of automatically generated tasks:

* Upload control documentation (evidence uploader)
* Review system configurations (tester)
* Validate test results (reviewer)

The test plan is now visible in the overview, and all participants can track progress through their task lists.

***

### Control Execution

{% embed url="https://vimeo.com/1074236399/f8cb57fe56" %}

Control Execution is the operational performance and documentation of a control. This can be a one-time activity or a recurring process managed through a Task Series.

#### Accessing Control Execution

1. Open the **Controls Workspace**
2. Select the control you want to execute
3. Navigate to the **Control Execution** tab
4. Review **Recent and upcoming** to see scheduled and completed executions

If no executions are scheduled, you'll need to create a Task Series.

#### Creating a Task Series

A Task Series automates the scheduling of recurring control executions. This ensures controls are performed consistently according to their designed frequency.

**How to Set It Up**

Click **Task Series** in the left menu to create a new series. You'll need to configure:

**Basic Information:**

* **Name:** Descriptive title (e.g., "Monthly Access Review" or "Quarterly Vendor Assessment")
* **Task type:** Select "Control execution"
* **Responsibles:** The person or team who will perform the control
* **Reviewers (optional):** Someone who validates the execution
* **Notifications:** Email or system alerts for upcoming tasks
* **Description:** Brief explanation of what needs to be done

**Planning Details:**

* **Repeat:** Choose the frequency (daily, weekly, monthly, yearly)
* **Repeat every:** Set the interval (e.g., every 3 months, every 2 weeks)
* **Repeat on:** Select the specific day or date
* **Start date:** When the task series begins
* **End date:** When the task series concludes (optional)

**Activation**

Click **save** to activate the task series.

Tasks will now automatically appear in the calendar of the responsible party at the specified frequency. Each execution is recorded in **All control executions** and can be tracked for audit purposes.

#### Why Task Series Matter

Task series ensure that:

* Controls are executed at their designed frequency
* Responsible parties receive automatic reminders
* Every execution creates an auditable record
* You can demonstrate consistent control operation to auditors

Without task series, control execution depends on manual tracking and individual memory, which is unreliable and difficult to prove.

***

### Effectiveness Testing

> {% embed url="https://vimeo.com/988376823/eb4cda568e" %}
>
> {% embed url="https://vimeo.com/988376852/fbaabd5d41" %}
>
> {% embed url="https://vimeo.com/988372284/15e696bb5d" %}
>
> {% embed url="https://vimeo.com/988376880/abfae0dff0" %}

Effectiveness Testing evaluates whether a control works in practice. This happens after the control has been executed, using real evidence from actual control operations.

#### Accessing Effectiveness Testing

1. Open the control from the **Controls Workspace**
2. Click on the **Effectiveness testing** tab

You'll see:

* An overview of existing test plans with status, period, sample count, documents, and scores
* Control details including description, frequency, linked risks, D\&I scores, and previous test results

#### Creating an Effectiveness Test Plan

**Step 1: Set Up Test Periods**

Click **Manage test periods** to establish the testing timeframe:

1. Define the period (e.g., calendar year, quarter, or custom range)
2. Determine how many samples will be tested
3. Click **save** to create the test period

An empty test period is now available and ready for test plan creation.

**Step 2: Add the Test Plan**

Click **Add test plan** and complete the following:

**Scope Definition:**

* Which control executions will be tested
* What evidence is required
* What constitutes effective operation

**Role Assignment:**

* Tester (performs the sampling and evaluation)
* Evidence uploader (provides supporting documentation)
* Reviewer (validates test conclusions)

**Instructions:**

* Clear guidance on what to test
* Expected evidence types
* Evaluation criteria

Click **save** to finalise the test plan. Workflow tasks are automatically generated and assigned.

#### Using the Audit Sampler

The **Audit sampler** button helps you generate statistically valid samples from source data.

**How It Works**

1. Click **Audit sampler** within your test plan
2. Choose the population type:
   * **Number of records** (e.g., 1,000 transactions)
   * **Date range** (e.g., all January executions)
   * **Excel upload** (import a population file)
3. Define how many samples need to be tested
4. The system randomly selects samples and assigns them to the test plan

The audit sampler ensures your testing is unbiased and defensible during audits.

#### Test Plan Status Tracking

The effectiveness testing overview shows real-time progress:

* **Status:** Current stage (e.g., "Waiting for evidence", "Testing in progress", "Under review")
* **#Samples:** How many of the planned samples have been tested
* **#Source documents:** Number of uploaded evidence files
* **Score:** Test outcome (sufficient / insufficient, effective / not effective)

As testers complete their work and upload evidence, these indicators update automatically. This visibility helps control owners and auditors understand testing progress without constant status meetings.

#### Test Results and Outcomes

A completed effectiveness test plan provides clear documentation:

* Which control was tested
* During which period
* Using which samples (specific instances of control execution)
* What the effectiveness score is (demonstrating whether the control works)

These results become part of your control assurance evidence and support audit and compliance activities.

***

### Exercises

#### Exercise 1: Design & Implementation Testing

1. Select a control from your organisation
2. Open the control and navigate to **Effectiveness testing** tab
3. Click **Manage test periods** and create a test period
4. Click **Add test plan** to create a D\&I test
5. Assign roles (tester, evidence uploader, reviewer)
6. Define scope and testing criteria
7. Click **save**
8. Verify the test plan appears in the list with status

> 💡 **Practice Tip:** Choose a control that's already documented so you can actually assess its design.

#### Exercise 2: Control Execution

1. Select a control that requires regular execution
2. Navigate to the **Control Execution** tab
3. Click **Task Series** in the left menu
4. Create a new Task Series:
   * Name: "Monthly \[Control Name] Execution"
   * Task type: Control execution
   * Responsibles: Assign to yourself or a colleague
   * Frequency: Monthly
   * Start date: Next month
5. Click **save**
6. Verify that planned executions appear in **Recent and upcoming**
7. Complete one execution and upload evidence (if in training environment)

#### Exercise 3: Effectiveness Testing

1. Use the same control from Exercise 2
2. Ensure some executions have been recorded (from Task Series)
3. Navigate to **Effectiveness testing** tab
4. Create a test period for the current quarter
5. Click **Add test plan** for effectiveness testing
6. Use **Audit sampler** to select samples from control executions
7. Assign a tester and reviewer
8. Upload at least one piece of supporting evidence
9. Complete the evaluation and assign a score (if in training environment)
