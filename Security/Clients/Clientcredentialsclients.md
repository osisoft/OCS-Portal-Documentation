---
uid: Clientcredentialsclients
---

# Client-credentials clients

Ignore this element.

Client-credentials clients are used for server-to-server communication where no user interaction is required. The client typically authenticates with the token endpoint using its client ID and secret. A secret is a unique key generated for each client, to connect to OSIsoft assets, resources and services for a limited period of time. Clients typically use two secrets so they can switch to the second secret before
the first expires.

**Training Video:** [Creating a Client Credentials Client](https://www.youtube.com/watch?v=JPWy0ZX9niU)

**NOTE:** You must have the role of Account Administrator to add and manage clients to your tenant.

## Manage client-credentials clients

* To create a new client-credentials client, click **Add Client** and complete the entry fields in the **Add Client** dialog box.

* To view or edit roles for a client, select an existing client, and click **Edit Client**.

* To remove a client, select an existing client, and click **Remove Client**.

## Manage secrets

* To create a new secret for a client, click **Add Secret** in the **Details** tab, and complete the entry fields in the **Add Secret** dialog box.

* To update secret details, select an existing secret and click **Edit Secret** in the **Details** tab.

* To remove a secret, select an existing secret and click **Remove Secret** in the **Details** tab.

## Manage roles for clients

* To view the assigned roles for a client, select an existing client, and click the **Roles** tab.

* To manage the roles for a client, select an existing client, and click **Manage Roles** in the **Roles** tab. Select the roles you want, and click **Save**.
