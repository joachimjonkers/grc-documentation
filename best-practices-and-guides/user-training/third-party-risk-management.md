# Third Party Risk Management

## Third Party Management

### Introduction

Third Party Management in CERRIX helps you register and monitor external vendors, suppliers, and service providers. This module provides centralized oversight of vendor relationships, ensuring proper risk management and compliance.

> 📹 **\[VIDEO PLACEHOLDER: Third Party Management Overview - 3 minutes]**
>
> * What Third Party Management is in CERRIX
> * How it connects to risks, controls, and data management
> * The review process and vendor lifecycle
> * Real example of managing a vendor

#### Why Use Third Parties in CERRIX?

Third parties introduce risks—operational dependencies, data protection concerns, compliance obligations. CERRIX Third Party Management provides:

* Centralized vendor registry
* Contract management with renewal tracking
* Review scheduling with automated reminders
* Risk and control linking
* GDPR Data Processor management
* Complete audit trail

#### How It Connects

Third parties integrate with:

* **Risks** – Document vendor-related risks
* **Controls** – Show vendor oversight controls
* **Data Management** – Track GDPR Data Processors
* **MoIs** – Address vendor issues
* **Documents** – Store contracts, DPAs, certifications

***

### Third Party workspace

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Third Party Workspace Overview]** Annotate:
>
> * "Third Party in navigation menu"
> * "List with columns: Identifier, Name, Review score (color-coded), Date reviewed, Next review date, Reviewer, Organisation responsible, Responsible"
> * "Add new Third Party button"
> * "Advanced configuration button"

The workspace shows all third parties with their review scores, dates, and responsible parties.

#### Review Score Indicators

* 🔴 **Red** – Poor/Bad (requires immediate attention)
* 🟡 **Yellow** – Fair (monitoring needed)
* 🟢 **Green** – Good/Excellent (performing well)

#### Filtering

> 📹 **\[VIDEO PLACEHOLDER: Filtering Third Party Workspace - 3 minutes]**
>
> * Using advanced configuration
> * Filtering by review score, organization, criticality
> * Creating and saving presets
> * Setting default views

Use filters to focus on:

* Vendors with poor review scores
* Vendors due for review
* Your department's vendors
* High-criticality vendors
* Data Processors (GDPR)

***

### Creating a New Third Party

> 📹 **\[VIDEO PLACEHOLDER: Creating a Third Party - 6 minutes]**
>
> * Complete walkthrough
> * Filling required vs optional fields
> * Setting up review schedules
> * Understanding Data Management roles
> * Saving and verification

#### How to Get There

1. Navigate to **Third Party** workspace
2. Click **Add new Third Party**
3. Complete the form

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Create Third Party Form - General Information]** Annotate:
>
> * "Name field (required)"
> * "Address, City, Country, Email, Phone, Website"
> * "Description field"
> * "EU member checkbox"

#### General Information

**Name** – Official company name (e.g., "Microsoft Corporation", "AWS")

**Basic details** – Address, city, country, email, phone, website

**Description** – What services does this vendor provide and why you use them

**EU member** – Important for GDPR data transfer considerations

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Create Third Party Form - Service Details]** Annotate:
>
> * "Status of involvement dropdown"
> * "Services multi-select"
> * "Start/End date servicing"
> * "Relationship dropdown"
> * "Criticality dropdown"

#### Service Details

**Status of involvement** – Active, Terminated, On hold, Under review

**Services** – Select services provided (IT Services, HR Services, Consulting, Data Processing, etc.)

**Start/End date servicing** – Contract period

**Relationship** – Supplier, Vendor, Partner, Contractor, Consultant, Processor

**Criticality** – High/Medium/Low (determines review frequency)

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Create Third Party Form - Internal Business]** Annotate:
>
> * "Organization responsible dropdown (required)"
> * "Responsible person"
> * "Organizations (in use) multi-select"
> * "Business/Framework dimensions"

#### Internal Business

**Organization responsible** – Which department manages this vendor (required)

**Responsible** – The individual who manages this relationship

**Organizations (in use)** – All departments using this vendor

**Business/Framework dimensions** – Link to processes and compliance frameworks

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Create Third Party Form - Data Management Roles]** Annotate:
>
> * "Data controller checkbox"
> * "Data processor checkbox"
> * "Data recipient checkbox"

#### Data Management Roles (GDPR)

**Data processor** – Vendor processes personal data on your behalf. **Most common for vendors handling customer/employee data.**

> ⚠️ **Important:** Data Processors require a Data Processing Agreement (DPA) under GDPR Article 28.

**Data controller** – Vendor determines purposes/means of processing (rare)

**Data recipient** – Vendor receives data for their own purposes

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Create Third Party Form - Contacts]** Annotate:
>
> * "Contact section with Add button"
> * "Contact form: Name, Role, Phone, Email"

#### Contacts

Add key contacts at the vendor (click **Add**):

* Primary contact for day-to-day
* Escalation contact for urgent issues

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Create Third Party Form - Review Information]** Annotate:
>
> * "Reviewer dropdown"
> * "Review frequency dropdown"
> * "Initial date"
> * "Next review date (auto-calculated)"

#### Review Information

**Reviewer** – Who conducts periodic vendor reviews

**Review frequency** – How often to review:

* Monthly – High-criticality vendors
* Quarterly – Medium-criticality
* Semi-annually / Annually – Lower-risk vendors

**Initial date** – When reviews start

**Next review date** – Auto-calculated from frequency

#### Saving

Click **Save third party** to create the vendor entry.

***

### Third Party Details

> 📹 **\[VIDEO PLACEHOLDER: Third Party Details Navigation - 3 minutes]**
>
> * Opening a third party
> * Left navigation menu
> * Details, Contracts, Links, History tabs
> * Editing and saving changes

When you open a third party, the left menu provides access to:

**🔹 Details** – View/edit all information

**📄 Contracts** – Manage contracts and renewals

**🔗 Links** – Connect to Risks, Controls, MoIs, Documents

**🔄 History** – View complete audit trail

***

### Managing Contracts

> 📹 **\[VIDEO PLACEHOLDER: Managing Contracts - 4 minutes]**
>
> * Adding a contract
> * Key fields: contract number, dates, value
> * Setting renewal reminders
> * Attaching contract documents

#### How to Get There

1. Open a third party
2. Click **Contracts** in left menu
3. Click **Add**

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Contracts Tab]** Annotate:
>
> * "Contracts tab selected"
> * "Add/Delete buttons"
> * "Contract list with details"

#### Key Fields

**Contract no.** – Reference number (e.g., "MSA-2025-001")

**Services** – What this contract covers

**Status** – Active, Expired, Pending, Terminated

**Currency & Value** – Contract amount

**Dates** – Signature date, contract date, end date

**Term of notice** – Notice period for termination

**Contract documents** – Attach signed contracts, DPAs, SLAs

> 💡 **Tip:** Set end dates accurately to receive renewal reminders and avoid missed renewals.

***

### Linking to Other Modules

#### Linking Risks

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Linked Risks]** Annotate:
>
> * "Links → Risks selected"
> * "List of linked risks"
> * "Risk identifiers and names"

Link vendor-related risks to show:

* Operational dependencies
* Data protection risks
* Security vulnerabilities
* Compliance obligations

**Common vendor risks:**

* "Cloud provider outage disrupts services"
* "Data processor security breach"
* "Vendor bankruptcy interrupts supply chain"

#### Linking Controls

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Linked Controls]** Annotate:
>
> * "Links → Controls selected"
> * "List of linked controls"

Link controls that manage vendor risks:

* Vendor due diligence processes
* Contract review and approval
* Quarterly security assessments
* Performance monitoring

#### Linking MoIs

Create improvement actions when issues arise:

* Failed security assessment → MoI to strengthen controls
* Missed contract renewal → MoI to implement tracking
* SLA breaches → MoI to address performance

#### Linking Documents

> 🖼️ **\[SCREENSHOT PLACEHOLDER: Documents Tab]** Annotate:
>
> * "Links → Documents selected"
> * "Add document button"
> * "Document list with download/edit options"

Upload vendor documentation:

* Contracts and amendments
* Data Processing Agreements (DPAs)
* Security certifications (ISO 27001, SOC 2)
* Insurance certificates
* Security assessments

***

### Review Process

#### Conducting Reviews

**1. Reviewer receives notification** when review is due

**2. Conduct assessment:**

* Check vendor performance vs SLAs
* Verify security certifications current
* Review any incidents
* Assess compliance with contracts
* For Data Processors: verify DPA is current

**3. Add review score:**

* Open the third party
* Scroll to **Review** section
* Click **Add**
* Enter date, score (Poor/Fair/Good/Excellent), and comments
* Save

**4. System calculates next review date** based on frequency

**5. Create MoIs** if issues are found

***

### Third Party User Roles

> 🖼️ **\[SCREENSHOT PLACEHOLDER: User Roles Matrix]** Show table from PDF with 7 roles and their permissions

#### Key Roles

**Third Party Unrestricted Administrator** – Full access, all organizations, manage standing data

**Third Party Restricted Administrator** – Full access, own organization only

**Third Party Unrestricted Writer** – Create/edit all third parties

**Third Party Restricted Writer** – Create/edit own organization only

**Third Party Viewer (Unrestricted/Restricted)** – Read-only access

**Third Party Reviewer** – Can only review assigned third parties

***

### GDPR Compliance

#### Data Processor Requirements

When a vendor is a **Data Processor**, GDPR Article 28 requires:

* ✅ Written Data Processing Agreement (DPA)
* ✅ Security measures documented
* ✅ Sub-processors authorized
* ✅ Data breach notification procedures
* ✅ Data return/deletion at contract end

#### Workflow

**In Third Party module:**

1. Mark vendor as "Data processor"
2. Attach DPA document
3. Schedule regular security reviews
4. Link to Data Management processing activities

**For GDPR audits:**

* Filter for all Data Processors
* Verify each has current DPA
* Show review history
* Demonstrate security assessments

***

### Best Practices

#### Registration

**Register vendors who:**

* Process data on your behalf (Data Processors)
* Have system/data access
* Provide critical services
* Pose regulatory risk

#### Documentation

**Always include:**

* Criticality level
* Review schedule
* At least two contacts
* Data processing role (if applicable)

**Attach:**

* Contracts
* DPAs (for Data Processors)
* Security certifications

#### Review Frequency

* **Monthly** – Critical vendors
* **Quarterly** – Important vendors
* **Semi-annually** – Standard vendors
* **Annually** – Low-risk vendors

#### Contract Management

* Track end dates
* Set term of notice
* Review 6 months before expiration
* Attach all contract documents

***

### Exercises

#### Exercise 1: Create a Third Party

1. Go to Third Party workspace
2. Click "Add new Third Party"
3. Create entry:
   * Name: "Microsoft Corporation"
   * Criticality: "High"
   * Organization responsible: Your department
   * Data processor: Checked
   * Review frequency: "Quarterly"
4. Save

#### Exercise 2: Add a Contract

1. Open your third party
2. Contracts → Add
3. Complete:
   * Contract no.: "MS-365-2026"
   * Status: "Active"
   * End date: One year from today
4. Save

#### Exercise 3: Conduct a Review

1. Open your third party
2. Review section → Add
3. Enter:
   * Date: Today
   * Score: "Good"
   * Comments: "Services performing well"
4. Save
5. Note next review date updated

***

**Next Module:** Continue to **Data Management** to learn about GDPR compliance and how Data Processors connect to processing activities.
