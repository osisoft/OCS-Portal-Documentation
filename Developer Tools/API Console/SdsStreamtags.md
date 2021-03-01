---
uid: SdsStreamtags  
---

# SdsStream tags

SdsStream tags are represented as a list of strings. SdsStream tags can
be used to categorize or denote special attributes of streams. Stream
tags can be used as criteria in search query strings to return SdsStream
results.

Following are some basic examples:

**GET /Namespaces/{namespaceId}/Streams/{streamId}/Tags**

Returns the tag list for the specified stream.

**PUT /Namespaces/{namespaceId}/Streams/{streamId}/Tags**

Replaces the tag list for the specified stream with the tags listed in the request body. Overwrites any existing tags; does not merge.

**DELETE /Namespaces/{namespaceId}/Streams/{streamId}/Tags**

Deletes the tag list for the specified stream.

See [SDS streams documentation and examples](https://ocs-docs.osisoft.com/Content_Portal/Documentation/SequentialDataStore/SDS_Streams.html).

