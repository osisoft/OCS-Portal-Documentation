---
uid: Dataviewdocumentation
---

# Data view documentation

A data view is a user selected subset of data stored in OSIsoft Cloud Services, mapped into custom tables. A data view includes data for use with a specific application or analysis, which is selected using a query for one or more data items.

A data item is a stream. Each column in a data view is mapped to a property of one or more data items. You can also organize data items into data groups within a data view in order for users to more easily compare similar properties in the same column.

| Keyword | Data Type | OCS Optionality | Description |
| ------- | --------- | --------------- | ----------- |
| Id | String | Required | Identifier for referencing the data view |
| Name | String | Optional | Name of the data view |
| Descriptions | String | Optional |     Description of the data view |
| DataFieldSets | IList | Optional |          List of Field Set items |
| GroupingFields | IList | Optional |          List of Field items |
| Shape | String | Optional | The shape of the data view |
| IndexField | Field | Optional | Index Field
| IndexTypeCode | SdsTypeCode | Optional |   Type of the Index Field |
| DefaultStartIndex | String | Optional |       Start Index |
| DefaultEndIndex | String | Optional |       End Index |
| DefaultInterval | String | Optional |        Interpolation Interval |

For usage examples, see the  [Data Views](https://ocs-docs.osisoft.com/Content_Portal/Documentation/DataViews/Data_Views_Overview.html) documentation.
