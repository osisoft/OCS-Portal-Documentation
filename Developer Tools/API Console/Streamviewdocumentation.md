---
uid: Streamviewdocumentation
---

# Endpoint / StreamViews

An **SdsStreamView** provides a way to map Stream data requests from one data type to another. You can apply a Stream View to any Read or GET operation. **SdsStreamView** is used to specify the mapping between source and target types.

SDS attempts to determine how to map properties from the source to the destination. When the mapping is straightforward, such as when the properties are in the same position and of the same data type, or when the properties have the same name, SDS will map the properties
automatically.

When SDS is unable to determine how to map a source property, the property is removed. If SDS encounters a target property that it cannot map to, the property is added and configured with a default value.

To map a property that is beyond the ability of SDS to map on its own, you should define an **SdsStreamViewProperty** and add it to the **SdsStreamView** properties collection.

The following table shows the required and optional **SdsStreamView** fields:

  | Property | Type | Optionality | Details |
  | -------- | ---- | ----------- | ------- |
  | id | String | Required | An identifier for referencing the stream view |
  | Name | String | Optional | Friendly name |
  | Description | String | Optional | Description text |
  | SourceTypeId | String | Required | Identifier of the **SdsType** of the **SdsStream** |
  | TargetTypeId | String | Required | Identifier of the **SdsType** to convert events to |
  | Properties | IList\<SdsStreamViewProperty\> | Optional | Property level mapping |

Following are some basic examples:

**GET/Namespaces/\[namespaceId\]/StreamViews**

Returns a list of stream views within a given namespace.

**GET/Namespaces/\[namespaceId\]/StreamViews/{streamViewId}**

Returns the stream view corresponding to the specified **streamViewId**
within a given namespace.

**GET/Namespaces/\[namespaceId\]/StreamViews/{streamViewId}/Map**

Returns the stream view map corresponding to the specified
**streamViewId** within a given namespace.

**POST/Namespaces/{namespaceId}/StreamViews/{streamViewId}**

Creates the specified stream view. SDS compares the stream view passed
in with existing stream views. If no matching identifier is found, SDS
creates the specified stream view. Click on **Insert View Template** to
auto-generate a stream view template in the body of the request.

**PUT/Namespaces/{namespaceId}/StreamViews/{streamViewId}**

Creates the specified stream view, if no stream view with the same Id
exists. If a stream view with the same Id already exists, the definition
of the stream view is updated. Click on **Insert View Template** to
populate the body of the request with the stream view specified by the
**streamViewId** in the path, if it exists. You can then edit properties
as desired.

**DELETE/Namespaces/{namespaceId}/StreamViews/{streamViewId}**

Deletes a stream view from the specified tenant and namespace.

For complete SDS stream view documentation and examples, click here.
