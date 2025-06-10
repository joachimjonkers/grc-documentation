# Authentication & User Provisioning

This page provides an overview of user provisioning and authentication options for CERRIX, leveraging Microsoft Azure Active Directory and Okta. It outlines the necessary steps and configurations to enable seamless user management and secure access to CERRIX applications.

The documentation is divided into three main guides, each addressing a specific aspect of integration:

* **Azure AD Authentication:** This section describes how to configure Azure Active Directory authentication for CERRIX. It covers the steps for app registration in Azure, including setting up the application name, redirect URI, supported account types, and implicit grant flow. It also outlines how to configure API permissions and provides the necessary information to CERRIX for application setup.

{% file src="../.gitbook/assets/CerrixAzureAdAuthentication 1.1.pdf" %}

* **User Provisioning using SCIM in Azure:** This section details the process of configuring user provisioning in Azure Active Directory using the System for Cross-domain Identity Management (SCIM) protocol. It covers creating an enterprise application, setting up initial connections, configuring attribute mappings for groups and users, and assigning the relevant groups for synchronization. Information required from CERRIX, such as the SCIM endpoint URL and a secret token, is also specified.

{% file src="../.gitbook/assets/UserProvisioningUsingScimInAzure.pdf" %}

* **User Provisioning using SCIM in Okta:** This section focuses on setting up user provisioning via SCIM through Okta. It guides users through creating an Okta app integration, configuring SAML settings, enabling SCIM provisioning, and mapping user attributes. Essential information from CERRIX, including the CERRIX URL and secret token, is highlighted.

{% file src="../.gitbook/assets/UserProvisioningUsingOktav1.0.pdf" %}
