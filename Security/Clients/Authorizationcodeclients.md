---
uid: Authorizationcodeclients
---

# Authorization code clients

Ignore this element.

Authorization Code Clients are used for customer web applications that use OSIsoft Cloud Services (OCS) as their backend. Authorization Code Clients provide a secure means of authenticating users of the website to view OCS assets. Creating an Authorization Code Client results in the generation of a Client ID, which must be specified in the web application using that Authorization Code Client to authenticate users.

Authorization code clients are used to authenticate using any browser, and an authorization code is provided to the client upon successful authentication. The authorization code is exchanged for an access token using PKCE (Proof Code for Code Exchange), which is a more secure authentication flow. No refresh token is provided.

**Training Video:** [Create an Authorization Code Client](https://www.youtube.com/watch?v=97QJjUKa6Pk&t=3s)

**NOTE:** You must have the role of Account Administrator to add and manage clients to your tenant.

* To create a new authorization code client, click **Add Client** and complete the entry fields in the **Add Client** window.

* To view or edit client roles, click on the name of an existing client, and click **Edit Client**.

* To remove a client, click on the name of an existing client, and click **Remove Client**.
