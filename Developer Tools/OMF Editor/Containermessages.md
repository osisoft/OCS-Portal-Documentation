---
uid: Containermessages
---

# Container messages

Container messages are used to create streams within the OCS Data Store.
To create a new stream an id and typeid are required as a minimum. The
id field is the Id that is assigned to the stream and the typeid is the
Id of the type that the new stream uses. The following is a list of
supported keywords:

| Keyword | Data Type | OCS Optionality | Description |
| ------- | --------- | --------------- | ----------- | 
| id | String | Required | Corresponds to the Stream Id field |
| typeid | String | Required | Corresponds to the Id of the type to be used by the stream |
| name | String | Optional | Data not grouped by containerid is not supported |
| description | String | Optional | Type versioning is not supported in OCS |
| tags | Array | Optional | An array of values used to help identify a stream |
| metadata | Object | Optional | Metadata key-value pairs |
| typeversion | String | Not Supported | Type versioning is not supported in OCS |
