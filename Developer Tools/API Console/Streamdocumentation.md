---
uid: Streamdocumentation
---

# Endpoint / Stream documentation

SDS stores collections of events and provides convenient ways to find and associate them. Events of consistent structure are stored in streams. An **SdsType** defines the structure of events in an **SdsStream**.

**SdsStreams** are referenced by their identifier or Id field, which must be unique within a namespace. An **SdsStream** must include a **TypeId** that references the identifier of an existing **SdsType**.

The following table displays required and optional **SdsStream** fields:

  | Property | Type | Optionality | Details |
  | -------- | ---- | ----------- | ------- |
  | Id | String | Required | An identifier for referencing the stream |
  | Type Id | String | Required |The **SdsType** to be used for this stream |
  | Name | String | Optional | The name of the stream |
  | Description | String | Optional | Text describing the stream |
  |Indexes | IList\<SdsStreamIndex\> | Optional | Used to define secondary indexes for the stream |

Following are some basic examples:

**GET/Namespaces/\[namespaceId\]/Streams**

Returns a list of streams within a given namespace.

**GET/Namespaces/\[namespaceId\]/Streams/{streamId}**

Returns the specified stream.

**GET/Namespaces/\[namespaceId\]/Streams/{streamId}/Type**

Returns the type definition that is associated with a given stream.

**POST/Namespaces/{namespaceId}/Streams/{streamId}**

Creates the specified stream. SDS compares the stream passed in with existing streams. If no matching identifier is found, SDS creates the specified stream. Click on **Insert Stream Template** to auto-generate a stream template in the body of the request.

**PUT/Namespaces/{namespaceId}/Streams/{streamId}**

Creates the specified stream, if no stream with the same Id exists. If a stream with the same Id already exists, the definition of the stream is updated. Click on **Insert Stream Template** to populate the body of the request with the stream specified by the streamId in the path, if it
exists. You can then edit properties as desired.

**DELETE /Namespaces/{namespaceId}/Streams/{streamId}**

Deletes a stream.

See [SDS Streams documentation and examples](https://ocs-docs.osisoft.com/Content_Portal/Documentation/SequentialDataStore/SDS_Streams.html).
