---
uid: Subscriptiondocumentation
---

# Subscription documentation

A subscription is used to consume data from a topic. Multiple
subscriptions can retrieve data from a single topic. There are two types of subscriptions with different behaviors.

**Standard subscription**

> A standard subscription provides an endpoint for an external > application to query. It maintains a bookmark into the topic queue and > serves up data in sequence. Standard subscriptions are not yet > supported.

**OCS Data Store subscription**

> An OCS Data Store subscription retrieves data from a topic and writes > it directly to a namespace in the OCS Data Store.
 
  | Property | Type | Optionality | Details |
  | -------- | ---- | ----------- | ------- |  
  | Id | String | Server-generated | Unique Id generated by the API during creation |
  | Name | String | Optional | A friendly name for the subscription |
  | TopicId | String | Required | Unique Id for the topic we are subscribing to |
  | TopicTenantId | String | Required | Identifies the owner of the topic |
  |TenantId | String | Required |Identifies the owner of the subscription |
  | NamespaceId | String | Required | Identifies the location of the subscription
  | Description | String | Optional | Description of the subscription |
  |CreatedDate |  String | Server-generated | The time that the subscription was created. The string is formatted using ISO 8601 format |
  | Enabled | Boolean | Server-generated | Whether the topic exists or not |

For complete usage examples, see the online documentation about Subscriptions - [OSIsoft, LLC](https://ocs-docs.osisoft.com/Content_Portal/Documentation/DataIngress/OMF_Ingress_Subscriptions.html).
