# Data Management

## Data Management

### Introduction

The Data Management module in CERRIX helps you register, manage, and assess data processing activities within your organisation. This is particularly important for GDPR (AVG) compliance and risk management related to data processing.

#### Purpose of the Data Management Module

Data processing activities need structured documentation to ensure:

* Compliance with data protection regulations
* Clear accountability for data handling
* Visibility into data flows and third-party processors
* Risk management around sensitive information
* Audit readiness and regulatory reporting

The Data Management module provides the framework for comprehensive data governance.

#### What You Can Do

* Register and classify processing activities
* Link processes to responsible parties, systems, and vendors
* Document privacy risks and control measures
* Export overview reports for audits or regulatory authorities
* Track data retention policies and legal bases
* Monitor third-party data processors

#### Benefits for Users

* One central overview of all data processing activities
* Traceability of data flows within the organisation
* Clear assignment of responsibilities for data protection
* Integration with risk and control frameworks
* Evidence base for GDPR compliance and audits

***

### Roles in Data Management

Multiple roles work together in CERRIX to keep data management information current and accurate.

#### Data Owner

The Data Owner is ultimately responsible for a data processing activity. They:

* Ensure registration accuracy and completeness
* Approve changes to processing activities
* Validate that legal bases are appropriate
* Oversee compliance with retention policies
* Make decisions about data usage and access

The Data Owner is typically a business function head or process owner, not someone from IT or legal.

#### Data Steward / Processor

The Data Steward collects and maintains processing details. They:

* Register new processing activities
* Keep information current and accurate
* Upload supporting documentation
* Link relevant risks, controls, or third parties
* Coordinate with Data Owners for approvals

Data Stewards are often the operational link between data users and governance teams.

#### Reviewer / Auditor

The Reviewer validates data management quality. They:

* Check completeness and consistency of registrations
* Assess compliance with internal and legal requirements
* Identify gaps or outdated information
* Recommend improvements to data governance practices

Reviewers provide independent oversight and help ensure data management doesn't drift from requirements.

#### Workflow Summary

**Data Steward registers → Data Owner approves → Reviewer validates periodically**

This structure balances operational efficiency with proper oversight and accountability.

***

### Data Management Workspace

The Data Management workspace provides an overview of all processing activities within your organisation.

#### What You See in the Workspace

Each processing activity is displayed with key information:

* **Processing purpose** – Name or description of the data processing activity
* **Owner** – The responsible person or department
* **Category of data** – Types of data being processed (personal, financial, sensitive)
* **Data subject** – Who the data relates to (customers, employees, suppliers)
* **Third party / Processor** – External parties involved in processing
* **Status** – Current state (Draft, Active, Under review, Closed)

#### Workspace Functions

**Advanced configuration** provides detailed filtering:

* Filter by status to see only active or under-review processing
* Filter by owner to see your own or your team's processing activities
* Filter by risk category to identify high-risk processing
* Filter by data subject type (e.g., show only employee data processing)

**Table configuration** controls which columns appear in the list. This helps focus on information relevant to your current task.

**Preset management** saves your filter and column configurations:

* Create presets like "My Processing Activities" or "High-Risk Processing"
* Set a default preset to load automatically when you open the workspace
* Share preset names with colleagues for consistent reporting views

#### Visual Indicators

Use colours and symbols to quickly identify:

* Processing activities requiring review or update
* High-risk processing needing additional oversight
* Recently added or modified entries
* Processing with missing required information

***

### Creating a New Data Processing Activity

#### How to Get Started

1. Click **Datamanagement** in the main menu
2. Click **Add processing purpose** in the top right corner

You'll be guided through capturing essential information about the processing activity.

#### Core Information

**Processing name** – A clear, descriptive name for the activity:

* Good: "Employee payroll processing"
* Good: "Customer credit card payment processing"
* Weak: "Processing activity 1"
* Weak: "Data management"

The name should immediately tell someone what data is being processed and why.

**Purpose** – The reason for processing this data:

* Payroll administration
* Customer relationship management
* Service delivery
* Contract performance
* Legal compliance
* Marketing and communications

Be specific about the business purpose. Vague purposes like "business operations" don't provide sufficient justification.

**Organisation / Business dimensions** – Link the processing to:

* The department or business unit responsible
* Relevant processes (e.g., HR processes, sales processes)
* Projects if the processing is temporary or project-specific

These connections help with reporting and accountability.

#### Data Categories

**Data categories** describe what types of data are being processed:

* Personal identifying information (names, addresses, IDs)
* Financial information (bank accounts, payment details)
* Employment information (salary, performance reviews)
* Health information
* Criminal records
* Biometric data
* Location data
* Online identifiers (IP addresses, cookies)

Select all categories that apply. Understanding what data you process is fundamental to GDPR compliance.

#### Data Subjects

**Data subjects** identifies whose data is being processed:

* Employees and job applicants
* Customers and prospects
* Suppliers and business partners
* Website visitors
* Children (requires special attention under GDPR)
* Other (specify)

Knowing your data subjects helps you apply appropriate protections and retention policies.

#### Legal Basis and Retention

**Legal basis** – The GDPR-compliant justification for processing:

* **Consent** – The individual has given clear consent
* **Contract** – Processing is necessary for contract performance
* **Legal obligation** – Processing is required by law
* **Vital interests** – Processing protects someone's life
* **Public task** – Processing is needed for a public interest task
* **Legitimate interests** – Processing is necessary for legitimate interests (with balancing test)

Choose the legal basis carefully. Each has different requirements and implications for data subject rights.

**Retention period** – How long data is kept:

* Specify duration (e.g., "7 years from contract end")
* Explain why this retention period is necessary
* Document the basis for the retention period (legal requirement, business need, industry standard)

GDPR requires you to not keep data longer than necessary. Document your retention decisions and implement them consistently.

#### Third Parties

**Third parties** identifies external organisations involved in processing:

* Cloud service providers
* Payment processors
* Marketing platforms
* Support service vendors
* Any processor who handles data on your behalf

For each third party, you should maintain:

* Data Processing Agreement (DPA)
* Assessment of their security measures
* Record of what data they access
* Notification if they experience a breach

#### Saving the Processing Activity

Click **Save** to create the processing activity. It now appears in the Data Management workspace and can be linked to risks and controls.

***

### Linking Risks, Controls, and Third Parties

Data processing isn't isolated – it connects to your broader risk management and vendor management programmes. These connections create a complete picture of data governance.

#### Linking Risks

1. Navigate to the **Linked risks** tab in your processing activity
2. Click to add or link risks
3. Select or create risks such as:
   * Data breach or unauthorised access
   * Data loss or corruption
   * Non-compliance with retention requirements
   * Excessive or inappropriate data collection
   * Third-party processor failures

These risk linkages help you:

* Understand what could go wrong with the processing
* Prioritise security investments
* Demonstrate risk-based data protection
* Connect data governance to enterprise risk management

#### Linking Controls

1. Navigate to the **Linked controls** tab
2. Add controls that mitigate data processing risks:
   * Encryption of personal data at rest and in transit
   * Access controls and authentication
   * Data backup and recovery procedures
   * Monitoring and logging of data access
   * Incident response procedures
   * Privacy by design controls

Linking controls demonstrates that you're not just documenting processing but actively protecting data.

#### Managing Third-Party Relationships

1. Navigate to the **Third parties** tab
2. Add or link external processors
3. For each third party, document:
   * Data Processing Agreement (DPA) or contract
   * Date of last security assessment
   * What data they access
   * What processing they perform
   * Their sub-processors (if applicable)
   * Incident notification procedures

Third-party management is a critical GDPR requirement. You remain responsible for data even when others process it on your behalf.

#### The Complete Picture

When you've linked risks, controls, and third parties, your processing activity becomes a comprehensive data governance record showing:

* What data is processed and why (legal basis)
* Who is responsible (data owner)
* What could go wrong (risks)
* What protections exist (controls)
* Who helps process the data (third parties)
* How long data is kept (retention)

This completeness is exactly what auditors and regulators want to see.

***

### Data Subject Rights and Impact Assessments

#### Data Subject Rights

When you process personal data, individuals have rights under GDPR:

* **Right to access** – Provide copies of their data
* **Right to rectification** – Correct inaccurate data
* **Right to erasure** – Delete data under certain conditions
* **Right to restriction** – Limit processing under certain conditions
* **Right to data portability** – Provide data in machine-readable format
* **Right to object** – Stop processing for certain purposes

Document in your processing activities:

* How you handle data subject requests
* Expected response times
* Who is responsible for responding
* What technical capabilities exist to fulfill rights

#### Data Protection Impact Assessments (DPIAs)

High-risk processing may require a DPIA under GDPR. Consider a DPIA when:

* Processing large amounts of sensitive data
* Systematic monitoring of public areas
* Processing data about vulnerable individuals
* Using new technologies
* Making automated decisions with legal effects

CERRIX can store DPIA documents linked to processing activities. This ensures impact assessments are readily available and integrated with risk management.

***

### Periodic Review and Updates

Data processing activities aren't static. Regular reviews ensure information remains accurate and compliant.

#### When to Review

Schedule reviews when:

* Legal bases or purposes change
* New third-party processors are added
* Data categories or subjects change
* Retention periods need adjustment
* Significant security incidents occur
* New regulations affect processing

We recommend annual reviews as a baseline, with more frequent reviews for high-risk processing.

#### Review Checklist

During reviews, verify:

* ✓ Processing description is still accurate
* ✓ Legal basis remains appropriate
* ✓ Data minimisation is applied (not collecting more than needed)
* ✓ Retention periods are justified and implemented
* ✓ Third-party agreements are current
* ✓ Linked controls are effective
* ✓ Data subject rights procedures are working
* ✓ No unauthorised changes to processing have occurred

Document review outcomes and any required updates.

***

### Best Practices

#### Be Specific in Descriptions

Vague processing descriptions don't meet GDPR requirements. Compare:

**Weak:** "We process customer data for business purposes"

**Strong:** "We process customer names, email addresses, and purchase history to fulfill orders, send shipping notifications, and provide customer support for 2 years after the last purchase"

The strong description explains what, why, and for how long – essential for transparency and compliance.

#### Use Data Minimisation

Only collect and process data you genuinely need. Before adding a new data category to a processing activity, ask:

* Is this data necessary for the stated purpose?
* Could we achieve the same purpose with less data?
* Are there privacy-preserving alternatives (aggregation, anonymisation)?

Data minimisation reduces risk and simplifies compliance.

#### Maintain Current Third-Party Registers

Out-of-date third-party information creates compliance risk. When a processor relationship changes:

* Update CERRIX immediately
* Ensure new DPAs are signed
* Assess new processors' security practices
* Document the change in the processing activity history

Don't wait for annual reviews to update processor information.

#### Link to Risk and Control Frameworks

Integrated governance is more effective than siloed systems. Connect data processing to:

* Risk registers (data protection risks)
* Control catalogues (data security controls)
* Incident management (data breach response)
* Audit programmes (data protection audits)

These connections demonstrate comprehensive data governance and reduce duplicate documentation.

#### Document Legal Bases Carefully

Choosing the wrong legal basis creates significant compliance risk. If unsure:

* Consult with legal or privacy professionals
* Document your reasoning for the chosen basis
* Be especially careful with "legitimate interests" – it requires a balancing test
* Remember that consent must be freely given and easily withdrawn

#### Keep Retention Policies Realistic

Don't arbitrarily set long retention periods "just in case." Justify retention with:

* Legal or regulatory requirements
* Business necessity
* Industry standards

Then implement the retention period with automated deletion or archiving.

***

### Exercises

#### Exercise 1: Create a New Processing Activity

1. Create a new data processing activity in the training environment
2. Complete all essential fields:
   * Processing name: Choose something realistic (e.g., "Employee performance review processing")
   * Purpose: Clear statement of why processing occurs
   * Organisation / Business dimensions: Link to a department
   * Data categories: Select relevant types
   * Data subjects: Who the data is about
   * Legal basis: Choose appropriately
   * Retention period: Specify duration and justification
3. Save the processing activity

#### Exercise 2: Link Risks and Controls

1. Open your newly created processing activity
2. Navigate to the **Linked risks** tab
3. Add at least one risk (e.g., "Unauthorised access to performance review data")
4. Navigate to the **Linked controls** tab
5. Add at least one control that mitigates the risk (e.g., "Role-based access control to HR system")
6. Verify the links are visible in the processing activity

#### Exercise 3: Conduct a Review

1. Select an existing processing activity (yours or a training example)
2. Review all fields for accuracy and completeness
3. Check that:
   * The processing description is still accurate
   * The legal basis remains appropriate
   * Retention periods are justified
   * Third-party information is current (if applicable)
4. Update the status if needed (e.g., mark as "Under review" while checking, then return to "Active")
5. Document any changes in the comments or notes section
