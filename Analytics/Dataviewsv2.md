---
uid: Dataviewsv2
---

# Data views

A data view is a user selected subset of data from one or more streams or assets.

You create a data view by defining the target namespace, the source stream(s) or asset(s), the desired data fields, time period, and interpolation interval. The ability to create data views in the portal will mesh directly with OSIsoft\'s Data Science Enablement efforts, whereby users will be able to programmatically access data view content via an API for the purposes of advanced analytics.

* To create a new data view, click **Add Data View** in the **Data Views** pane, and then enter the data view **Name** and **Description**.

* Type an identifier in the **Query ID** field. In the **Query Type** area, click either the **Streams** or **Assets** button.

* For data streams: Type a portion of the name of any known stream (preceded/followed by the \* wildcard symbol) in the **Find Streams** window and click **Apply** to retrieve streams matching your criteria.

* For assets: Type a portion of the name of any known asset (preceded/followed by the \* wildcard symbol) in the **Find Assets** window and click **Apply** to retrieve assets matching your criteria.

* Select the data fields, time period, and the interpolation interval required for the new data view.

* To set permissions for a data view, select an existing data view and then click **Manage Permissions**. You select **Allow** or **Deny** for each of the following permissions: **Read**, **Write**, **Delete**, and **Manage Permissions**, for each role you select from the **Selected role** drop-down list.

* To edit a data view, select an existing data view, and then click **Edit Data View**.

* To delete a data view, select an existing data view and then click **Remove Data View**.
