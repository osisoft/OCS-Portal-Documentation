---
uid: metadatarules
---

# Metadata rules

OSIsoft Cloud Services Metadata rules enable you to relate similar data streams for the purposes of analysis and display, and to feed into downstream applications. Metadata rules also create and assign metadata to the streams they identify. You create metadata rules by selecting parsable metadata from stream name structure, and applying the rule to identify streams whose names match the defined pattern. OCS parses streams based on the selected stream name pattern you designate in your rule.

**Training Video:** [Create a metadata rule](https://www.youtube.com/watch?v=641Q3YRzEFE)

You can create metadata rules for streams only. In the Metadata rules page of the OCS portal, you can add, edit, or delete metadata rules for streams. It is advisable to take existing or planned metadata rules into consideration when creating streams, as well as to add metadata as it becomes available or changes. Stream names which follow a standard pattern, including items such as location, asset class and asset Id in the name are more applicable to the creation and use of metadata rules.

For example, you might define a location, facility, asset class, or asset Id as metadata by which to group streams. These metadata typically correspond to properties of the type on which the targeted streams are based. In this scenario, you might define a metadata rule to identify all streams for oil pumps in Phoenix, operating in a specific facility.

*	To create a new metadata rule, click **Add Metadata Rule** in the **Metadata Rules** pane, and then type a portion of the name of any known stream in the **Select Stream** window. Click the stream name you want to use for your rule criteria, and click **Next**.
  
  *	You designate each delimited section of the selected stream name as Metadata, String Literal, or Wildcard. Streams matching your rule will be assigned the metadata you define in this step.
  
  *	You can create mappings for the sections of the stream name that you designate as metadata, which enables you to display the full name of a location or facility rather than its code, for example.
  
*	To set permissions for a metadata rule, select an existing rule and then click Manage Permissions. You select **Allow** or **Deny** for each of the following permissions: Read, Write, Delete, and Manage Permissions, for each role you select from the Selected role drop-down list.

The value of metadata itself lies in its capacity to enrich sequential data, and to facilitate logical segregation and contextualization of data. Metadata rules enable the bulk creation and maintenance of stream metadata, which can then be used across OSIsoft Cloud Services. Other services and applications, such as OCS data views, leverage stream metadata to simplify finding data and to provide context about stream data.

For more information, see [Add context with metadata rules](xref:addcontextwithmetadatarules).
