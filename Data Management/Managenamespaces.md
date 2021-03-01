---
uid: Managenamespaces
---

# Manage namespaces

An SDS tenant is divided into one or more namespaces. Namespaces may correspond to a specific set of infrastructure assets, but more commonly correspond to virtual partitions within a single set of assets. Each namespace corresponds to an instance of SDS, and holds its own set of SDS Types, SDS Streams, and SDS Stream Views. Namespaces serve as the
destination for incoming stream data.

Namespace Ids are subject to the following requirements:

  * Must contain 260 characters or fewer

  * Must only contain alphanumeric characters, underscores, dashes, spaces, and periods

  * Must not contain two consecutive periods

  * Must not start or end with a period

  * Must not start with two consecutive underscores

  * To create a new namespace, click **Add Namespace** and complete the entry fields in the **Add Namespace** window. After entering a **Namespace Id** and **Description**, you can select a region for the new namespace from the **Region** drop-down list, if multiple regions are available for your tenant. The field is pre-populated if only one region is available.         |
   
**NOTE:** You cannot change the region for a namespace after you have created it.

  * To manage permissions for a namespace, select an existing namespace, and click **Manage Permissions**.                    

  * To edit a namespace, select an existing namespace, and click **Edit Namespace**. When editing a namespace, recall that the Namespace Id must be unique within your tenant. When finished editing the namespace, click **Save**.

  * To view namespace details, select an existing namespace, and click **Display Details**. The type count, stream count, and behavior count fields refer to the number of types, streams, and behaviors that have been created for the selected namespace.
  
  * To remove a namespace, select an existing namespace, and click **Remove Namespace**.

