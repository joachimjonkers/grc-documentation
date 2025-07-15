# How to Create an Anonymous Form (e.g. for Whistleblowing)

{% hint style="danger" %}
This tutorial is only valid starting with the release of July 15th (ACC) and August 12th (PRD)
{% endhint %}

In some use cases—such as whistleblowing—it’s essential to collect information anonymously. CERRIX allows for the creation of anonymous form submissions by using an API-based approach that is not linked to any specific user account.

This guide walks you through setting up such a form and enabling anonymous submission via the CERRIX API.

***

## Step 1: Create the Form

1.  Go to the Forms module

    From your CERRIX dashboard, navigate to Forms in the main navigation menu.
2.  Click “Add new form”

    This opens the form builder interface.
3.  Define form fields

    Add the fields you want respondents to fill out. This can include text fields, dropdowns, attachments, etc.
4. Optional: Add information for respondents explaining that submissions are anonymous.
5.  Publish the form

    A form must be opened for responses before you can submit responses via the API.
6. Note down the form ID, which can be found by copying the URL of the form page.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

***

## Step 2: Generate an API Key

1.  Open your user profile

    Click on your name in the top-right corner and select API Keys.
2. In the left-hand menu, click "API Keys"
3. Click “Add API Key”
4. Select the right permission
   *   Choose the permission: create form result

       This allows the API key to submit entries to the selected form.
5.  Restrict by IP address

    For security reasons, specify the IP address or IP range that will be allowed to use this key.
6.  Save your API key

    Copy the key somewhere secure—you will not be able to view it again.

***

## Step 3: Submit Anonymous Entries via API

Once your form is published and you have a valid API key, you can start submitting entries without linking them to a CERRIX user.

Refer to the Create Form Result description in the CERRIX API Manual for the exact request format.

This API enables anonymous submissions, but it should be embedded within a frontend form or tool—such as a website or internal portal—that whistleblowers or other users can interact with directly.
