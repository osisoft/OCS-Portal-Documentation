---
uid: Identityproviders
---

# Identity providers

Ignore this element.

An identity provider is a third-party service that stores and
authenticates users.

**NOTE** You must have the role of Account Administrator to add and manage the identity provider for your tenant.

To add a new identity provider, take the following steps:

  1. Select the identity provider you want to activate from the list of identity providers supported on your tenant.

  2. Click **Activate** in the **Details** tab. A message prompts you to confirm that you want to activate a new identity provider for the tenant.

  3. Click **Activate** in the message window.
  
  4. Specify the role(s) to assign to this new group.

  5. If you selected Azure Active Directory, an Add Identity Provider window appears where consent is configured.

To add an identity provider that supports advanced integration, such as Azure Active Directory, you must obtain consent from that tenant\'s Administrator:

  1. Enter the Azure Active Directory\'s Tenant ID or Domain Name of that identity provider.

  2. Select the Enable Advanced Integration checkbox.

  3. Enter the Azure Account Administrator\'s email address.

  4. Enter the Azure Account Administrator\'s name.

  5. Click **Request Consent**.

If the identity provider shows a status of **Inactive; Pending
Consent**, you must obtain a consent from this identity Provider to perform advanced integration with your tenant:

  1. Click **Edit Consent**.

  2. Enter the Azure Active Directory\'s Tenant ID or Domain Name if not already specified.

  3. Select the **Enable Advanced Integration** checkbox if not already selected.

  4. Enter the Azure Account Administrator\'s email address.

  5. Enter the Azure Account Administrator\'s name.

  6. Click **Request Consent**.
  
  **NOTE:** You can only add identity providers. Once you have enabled an identity provider for your tenant, it cannot be deactivated for that tenant.
