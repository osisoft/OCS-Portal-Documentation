---
uid: SdsStreammetadata
---

# SDS Stream Metadata

Sds Stream Metadata is represented as a dictionary of string keys and associated string values. It can be used to associate additional information with a stream. Stream metadata can be used as criteria in search query strings to return SdsStream results.

Some basic examples:

**GET /Namespaces/{namespaceId}/Streams/{streamId}/Metadata**

Returns the metadata dictionary for the specified stream.

**GET /Namespaces/{namespaceId}/Streams/{streamId}/Metadata/{key}**

Returns the value for the specified key in the metadata dictionary of the specified stream.

**PUT /Namespaces/{namespaceId}/Streams/{streamId}/Metadata**

Replaces the metadata for the specified stream with the metadata in the request body. Overwrites any existing metadata; does not merge.

**DELETE /Namespaces/{namespaceId}/Streams/{streamId}/Metadata**

Deletes the metadata for the specified stream.

For complete SDS streams documentation and examples, click here.

See [SDS Stream Metadata and Tags](https://ocs-docs.osisoft.com/Content_Portal/Documentation/SequentialDataStore/SdsStreamExtra.html)