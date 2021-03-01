---
uid: Typemessages
---

# Type messages

The following is a description of keywords and what is supported to
compose a type message for OCS consumption:

| Keyword | Data Type | OCS Optionality | Description |
| ------- | --------- | --------------- | ----------- |
| id | String | Required | Corresponds to the **Type Id** field |
| classification | String | Required | Can be either dynamic or static. OCS only supports dynamic |
| type | String | Required | Inherited from JSON schema. Must be set to object |
| properties | Object | Optional | Key-value pairs defining properties of the Type |
| \*\*type | String | Required | Each key of type properties defines an object that must contain the type property |
| \*\*format | String | Optional | Format for the type property |
| \*\*isindex | Boolean | Optional | Determines if the property is an index for the type, and corresponds to the iskey attribute of a type property in OCS |
| name | String | Optional | Friendly name for the type |
| description | String | Optional | A description for the type |
| tags | Array | Not Supported | Currently unsupported in OCS |
| metadata | Object | Not Supported | Currently unsupported in OCS |
| version | String | Not Supported | Currently unsupported in OCS |

\*\* type, \*\*format and \*\*isindex are keywords for the object
defined by each key-value pair of properties. Example:
```
\"properties\": {
  \"EXAMPLE_PROPERTY\": {
    \"type\": \"integer\",
    \"format\": \"int64\",
    \"isindex\": true
  }
}
```