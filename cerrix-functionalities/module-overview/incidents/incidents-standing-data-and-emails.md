# Incidents Standing Data & Emails

The Incident Standing Data functionality in CERRIX enables users to define and manage reusable data components used when creating and handling incidents. This feature provides flexibility, control, and customization tailored to your organization's specific incident management needs.

This documentation explains how to manage Incident Standing Data, including classifications, incident types, custom fields, and email notifications in CERRIX’s Incident Management module.

{% embed url="https://vimeo.com/1093634626" %}

***

## Accessing Incident Standing Data

Incident Standing Data is located within the **Incident Workspace** in CERRIX.

1. Navigate to **Incidents** from your main menu.
2. On the Incident Workspace, locate and click on the **Standing Data** in t
3. he left hand menu.

<figure><img src="../../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

***

## Managing Classifications

Classifications define the severity or urgency level of an incident (for example: Low, Medium, High).

#### To manage classifications:

1. Within the **Standing Data** menu, select **Classification**.
2. Modify or add new classifications:
   * Change the name of existing classifications.
   * Apply a color code to quickly visualize severity.

<figure><img src="../../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

***

## Managing Incident Types

Incident Types allow you to define and tailor the data fields specifically needed when users log incidents.

#### Creating an Incident Type

To create a new incident type:

1. Within **Standing Data**, click on **Incident Types**.
2. Select **Add**.
3. Enter a descriptive name to identify the Incident Type clearly.

<figure><img src="../../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>

### Adding Custom Fields

You can add custom fields to any new incident type:

1. **Create Sections** to logically group custom fields:
   * Name and rearrange sections easily.
   * Remove fields and sections as needed.
2. **Add Fields** within sections:
   * Fields can be configured by:
     * Field Type: Text field, Text area, Date, Date-Time, Number, Checkbox, Dropdown single select, Dropdown multi select, Financial impact.
     * Name
     * Placeholder (optional)
     * Instruction guide text (optional)
     * Visibility status (visible/hidden)
     * Required status (mandatory/optional)
   * Adjust whether fields are required or optional.

**Examples of Adding Custom Fields:**

* **Text area field:** Provide open-ended text inputs.
* **Drop down single select:** Let users select from a predetermined list. Colors can be optionally assigned per choice.
* **Financial Impact:** Numerical data or specific values tailored to your incident reporting needs.

<figure><img src="../../../.gitbook/assets/image (18).png" alt=""><figcaption></figcaption></figure>

### Configuring Email Notifications

Incident types can trigger notifications to specific recipients upon creation.

To configure notifications per incident type:

1. Select your incident type.
2. Navigate to the **Configuration** tab.
3. Add email address(es) for recipients who need notification when an incident with this type is created.

<figure><img src="../../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

***

## Standard (Built-in) Incident Types

CERRIX provides two pre-defined incident types for common use cases:

* **Operational Incident**
* **Data Breach**

These built-in incident types:

* Cannot be edited or deleted.
* Guarantee compatibility with pre-established forms and reporting structures.
* Maintain existing data mappings and integration points.

> **Important:** Custom fields cannot yet be added to standard types (e.g., Data Breach). However, this enhancement will be available in future updates.

### DORA Incident Types

As part of CERRIX’s support for the Digital Operational Resilience Act (DORA), a standardized set of DORA-specific incident types is now available. These incident types are aligned with the reporting obligations under DORA and are designed to help organizations track and report major ICT-related incidents effectively.

#### Overview

The DORA incident types are provided as a predefined template in the system. These are separate from your custom incident types and follow the structure required for DORA-compliant reporting.

#### Available in the Following Report Types

The DORA incident fields and structure are embedded in three predefined report types:

* DORA Initial Report
* DORA Intermediate Report
* DORA Final Report

These templates ensure that incident reporting aligns with regulatory expectations throughout the incident lifecycle.

#### Key Features

* Standardized Structure: Includes all fields required for DORA reporting (e.g., incident classification, root cause, impact, response timeline).
* Pre-filled Field Labels: Uses terminology aligned with regulatory guidelines to ensure consistency.
* Integration Ready: Templates are structured for easy integration with external DORA reporting systems.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Incident Sent Emails

As an administrator, all sent mails can be viewed via an extra tab in the incident module, underneath the Standing Data.

<figure><img src="../../../.gitbook/assets/image (2) (1) (2) (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (3) (1) (2) (1).png" alt=""><figcaption></figcaption></figure>
