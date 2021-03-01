---
uid: APIconsole
---

# API console

The API Console provides a graphical interface to utilize the SDS REST API, which enables you to read and write SDS data. Complete the following to utilize the API Console:

  1. Select an action from the **GET/POST/PUT/DELETE** droplist.
  
  2. The search window displays **Namespaces** by default. Type a backslash (/) after **Namespaces** to display a droplist of available namespaces.

  3. Select the name of the specific namespace to/from which you want to read/write data.
  
  4. Click the blue button in lower right (button label is the action you selected in Step 1).

The API Console provides a graphical interface to utilize the SDS REST API, which enables you to read and write SDS data. To use the API Console, you select a GET, POST, PUT, or DELETE action, select the desired objects for the action, and execute.

Each request begins with an HTTP verb (GET, POST, PUT,DELETE) and is followed by a path to the appropriate SDS REST endpoint./api/tenants and your tenant ID are automatically prepended to the path you enter. You
will then need to append /{namespaceId} to /Namespaces in the URI field, and append to that the desired endpoint.

**Result:** The request to /Streams endpoint will be issued to SDS as /api/Tenants/{tenantId}/Namespaces/{namespaceId}/Streams. The complete path displays in the **Full Path** field of the **API Console**. For **POST** and **PUT** requests, the **Body** entry field displays. Type the request body into the **Body** entry field.

For more information, see [API calls for reading data](https://ocs-docs.osisoft.com/Content_Portal/Documentation/SequentialDataStore/Reading_Data_API.html).
