---
uid: Datamessages
---

# Data messages

Data messages are composed of an array of objects to be written to the
stream specified by the containerid. The objects must conform to the
type with which the container is associated. The following is a list of
supported keywords:

| Keyword | Data Type | OCS Optionality | Description |
| ------- | --------- | --------------- | ----------- |
| containerid | String | Required | Corresponds to the **Stream Id** field |
| values | Array | Required | An array of values to be written to the stream |
| typeid | String | Not Supported | Data not grouped by containerid is not supported |
| typeversion | String | Not Supported | Type versioning is not supported in OCS |
