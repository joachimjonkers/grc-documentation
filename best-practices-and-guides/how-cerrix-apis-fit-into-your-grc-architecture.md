# How CERRIX APIs fit into your GRC architecture

CERRIX is designed as a **modular and open GRC platform** that integrates seamlessly into your organization’s existing IT, risk, finance and audit landscape.

Most organizations already operate dozens of systems that contain relevant governance, risk and compliance data: IT service management, finance, HR, identity, vendor platforms, monitoring tools, and audit software. To establish effective, auditable and scalable GRC, this data must be exchanged in a **secure, structured and automated** way.

CERRIX uses APIs across all core modules to make this possible.

These APIs allow CERRIX to act as the **central system of record for GRC**, while data continues to flow between operational systems, reporting tools, auditors and regulators.

## What CERRIX APIs are used for

CERRIX APIs support a wide range of GRC use cases. Together, they enable automation, data consistency and continuous assurance across the entire GRC lifecycle.

### Data extraction for reporting and analytics

CERRIX provides APIs across all core modules, including:

* Risks
* Controls, tasks and tests
* Improvement actions
* Incidents
* Third parties

These APIs allow organizations to extract data into external systems such as:

* Business intelligence tools
* Data warehouses
* Audit and assurance tooling

This enables CERRIX to function as the **single source of truth for GRC data**, while reporting and analysis can be performed in the organization’s preferred tools.

In addition to module-specific APIs, CERRIX offers combined APIs that retrieve data across multiple modules in one request. For example:

* Risks, controls and improvement actions in relation to each other
* Incidents linked to underlying risks and controls

This supports integrated reporting and makes it easier to demonstrate how risks, controls and follow-up actions are connected.

All reporting and extraction APIs use **GET** requests.

### User provisioning and access governance (SCIM)

CERRIX supports automated user provisioning and authorization management through **SCIM** integrations with enterprise identity platforms.

This allows organizations to:

* Automatically create and update users
* Assign the correct profiles and roles
* Enforce joiner, mover and leaver processes

Using SCIM significantly reduces manual administration, minimizes the risk of incorrect access, and strengthens auditability of user management.

### Control assurance through automation

CERRIX supports both automated control testing and continuous control monitoring through APIs.

#### Automated control testing

For quantitative controls, CERRIX can independently generate test samples from a defined population. APIs are used to automate this workflow:

* The population is provided through an integration
* CERRIX generates a sample
* The selected items are returned to the source system
* Evidence is retrieved and automatically stored in CERRIX

This removes manual sampling, reduces administrative work, and ensures that testing is objective, reproducible and fully auditable.

Both **GET** and **POST** APIs are used in this process.

#### Continuous control monitoring

For quantitative controls, CERRIX can independently generate test samples from a defined population. APIs are used to automate this workflow:

* The population is provided through an integration
* CERRIX generates a sample
* The selected items are returned to the source system
* Evidence is retrieved and automatically stored in CERRIX

This removes manual sampling, reduces administrative work, and ensures that testing is objective, reproducible and fully auditable.

Both **GET** and **POST** APIs are used in this process.

### Third-party and external audit assurance

CERRIX supports external auditors through API-based Third Party Assurance.

Using APIs, an external audit firm can securely connect its tooling to the customer’s CERRIX environment and access:

* Risks
* Controls
* Test results
* Improvement actions

This removes the need for manual preparation steps such as:

* Delivering control overviews
* Compiling audit evidence
* Aligning scopes and definitions

As a result, audits become faster, more consistent and more reliable.

These integrations primarily use **POST** APIs.

You can read more about External Connections for Third Party Assurance here: [external-connections.md](../cerrix-functionalities/admin-settings/external-connections.md "mention")

### Automated data collection for KRIs and KPIs

CERRIX includes a KRI and KPI module for monitoring risk indicators and performance metrics against thresholds and risk appetite.

The data required for these indicators often comes from multiple source systems, such as:

* IT service management
* Finance
* HR
* Security tooling

Through APIs, this data can be delivered automatically to CERRIX, allowing:

* Continuous updates of KRIs and KPIs
* Near real-time visibility of deviations
* Elimination of manual data entry errors

This supports data-driven risk management and timely escalation.

These integrations use **POST** APIs.

### Incident and whistleblower reporting

Within the CERRIX Forms module, APIs are available for submitting form data directly from external systems.

This enables use cases such as:

* Automatic registration of priority-1 IT incidents from an ITSM tool
* Secure receipt of anonymous whistleblower reports from external reporting channels

By receiving these reports via APIs, CERRIX can immediately:

* Register the incident
* Link it to relevant risks and controls
* Trigger follow-up actions

These integrations use **POST** APIs.

### Third-party risk management and supplier data

CERRIX supports the registration and monitoring of suppliers, with specific focus on critical and outsourced parties.

Many organizations already maintain supplier data in dedicated vendor management systems. From Q1 2026, CERRIX will support synchronization of supplier data through APIs, enabling:

* A single source of truth for supplier information
* Automated monitoring of supplier risks and controls
* Up-to-date and consistent vendor data

This supports regulatory requirements such as **DORA, NIS2 and outsourcing regulations**.

These integrations use **POST** APIs.

## Technical principles

### REST-based architecture

All CERRIX APIs are implemented as **REST APIs** using standard web technologies. This ensures that integrations are:

* Lightweight
* Scalable
* Secure
* Easy to implement with existing IT tooling

This approach fits naturally into modern enterprise architectures.

### No rate limiting

CERRIX APIs are designed for enterprise-grade usage. No rate limiting is applied, allowing organizations to:

* Run continuous synchronizations
* Perform large-scale reporting and exports
* Support high-volume automation and auditing

This makes the APIs suitable for both operational and analytical use cases.
