---
uid: Users
---

# Users

A user is an identity that has access to OSIsoft assets, resources and services. The role assigned to the user helps determine what the user can do on the resource. Users may be assigned one or more roles, but all users are assigned the Account Member role by default.

**NOTE:** You must have the role of **Account Administrator** to add and manage users to your tenant.

To view the roles assigned to a specific user, select the user. The list of roles for that user appears in the **Roles** tab.

To add a new user:

  1. Click **Add User**.

  2. Select an identity provider to authenticate the user. Whether the selected identity provider supports advanced integration determines the next steps.

  3. If you select Google or Microsoft, basic integration is supported only, where you specify a user to invite.

      1. Enter the first name, last name, and the contact email of the new user. 

      2. Select the roles to assign to the new user.           

      3. Click **Invite**. The invited user receives an email invitation to accept access to OSIsoft assets, resources and services. The user must accept this invitation for them to show as a user to the tenant. |

  4. If you select Azure Active Directory, advanced integration is supported, where you are able to search for a user to add from a directory. Advanced integration is available after the AAD tenant consented during the setup. Otherwise, you must specify a user to invite with basic integration. 
  
      1. Enter the name or the email address of the user to initiate the search of that user.

      2. Select the user from the search drop down.            
      
      3. Select the roles to assign to the new user.           
      
      4. Click **Add**. The user receives a notification that they were added to the OSIsoft tenant.

To update an existing user, click **Edit User**. You can modify the identity provider, contact information and email and assigned roles for this user.

**NOTE:** For AAD users added through advanced integration, you can only modify the roles. However, if basic integration is used, you can modify user properties for users as well as roles.

To resend an invitation to a Microsoft or Google user, click **Resend Invitation**.

To remove an existing user, click **Remove User**.

**NOTE:** You cannot remove the current user tenant.

