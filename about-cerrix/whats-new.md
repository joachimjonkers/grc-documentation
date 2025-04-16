# What's New?

## Release notes

### March 2025

#### **Third party**

**LEI code**

It is now possible to register the LEI code of a third party including a LEI code validity check. The LEI code is available in the workspace and API.

#### **Audit**

**Audit sponsor**

In an Audit, the Sponsor or Sponsors, can now be registered. The Sponsor could be, for instance, the initiator of the audit. The sponsor does not have any rights, not even view rights. In the document templates the field Sponsor(s) can be added.

#### **Risk**

**Budget-based risk scoring**

A new way of scoring risks has been made available. Budget-based risk scoring is the first set-up for this initiative. The purpose is to enable risk scoring based on an estimated financial impact in relation to an organizational budget.

This feature is still experimental. If you are interested, please submit a ticket in the Customer Portal.

{% content-ref url="../cerrix-functionalities/module-overview/risks/budget-based-risk-scoring.md" %}
[budget-based-risk-scoring.md](../cerrix-functionalities/module-overview/risks/budget-based-risk-scoring.md)
{% endcontent-ref %}

### February 2025

#### **Workspace preset hyperlink**

**Hyperlinks for public presets**

It is now possible in the Browse presets overview to create a link to a preset. If the preset is public, this link can be shared with other users via mail or messaging tool for instance. Please be aware that this is only possible for presets that are made public.

#### **Notable fixes**

**User management - Role group removal does not lead to removal of the associated roles for the user**

Role group removal did not lead to removal of the corresponding roles of the user. This issue has now been solved. After removing a role group for a user, the corresponding roles are removed for the user if no other active rolegroup for that user includes that role.

### January 2025

#### **Notable fixes**

**KRI - KRI restricted writer can't edit KRI datapoints**

KRI restricted writer could not edit KRI datapoints

**Audit - Unassigned Auditee cannot be requested to provide a document**

All users with the role Auditee could be asked via a mail request defined in the Audit to supply information to an audit. However, only users assigned to an Audit have the rights to do so. In this release both have been aligned: only Auditees assigned to the Audit can be asked to add information to an audit.\
