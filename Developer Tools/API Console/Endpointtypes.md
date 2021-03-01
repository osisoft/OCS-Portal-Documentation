---
uid: Endpointtypes
---

# Endpoint / Types 


**SdsTypes** can define simple atomic types, such as integers, floats, strings, arrays, and dictionaries, or they can define complex types using **SdsTypes**. You can define complex, nested types using the Properties collection of an **SdsType**.

An **SdsType** used to define an **SdsStream** must have a **Key**. A **Key** is a **Property** or a combination of **Properties** that constitute an ordered, unique identity. The **Key** is ordered, so that it functions as an **index**; it is known as the **Primary Index**.

While a **timestamp** (DateTime) is a very common type of **Key**, any type that can be ordered can be designated as the **Primary Index**.

When defining a type, consider how the events will be represented in a stream. The **SdsType** defines each event in the stream. Each event is a single unit whose properties have values that relate to the index, and each property of an **SdsType** event is related to the event's index.

An **SdsType** is referenced by its identifier or Id field. **SdsType** identifiers must be unique within a Namespace.

The following table shows the required and some optional **SdsType** fields.

  | Property | Type | Optionality | Details |
  | -------- | ---- | ----------- | ------- |
  | id | String | Required | An identifier for referencing the type |
  | Name | String | Optional | Name |
  | Description | String | Optional | Text that describes the type |
  | SdsTypeCode | SdsTypeCode | Required | Defines the type
  Properties | IList | Required | List of SdsTypeProperty items


Following are some basic examples:

**GET/Namespaces/[namespaceId\]/Types**

Returns a list of types within a given namespace.

**GET/Namespaces/[namespaceId\]/Types/{typeId}**

Returns the type corresponding to the specified typeId within a given namespace.

**POST/Namespaces/[namespaceId\]/Types/{typeId}**

Creates the specified type. SDS compares the type passed in with existing types. If no matching identifier is found, SDS creates the specified type. Click on **Insert Type Template** to auto-generate a type template in the body of the request.

**Note:** You cannot edit an existing type. In order to have a type with different properties than originally assigned, you must create a new type.

**DELETE/Namespaces/{namespaceId}/Types/{typeId}**

Deletes a type from the specified tenant and namespace.

**Note:** A type cannot be deleted if any streams, stream views or other types reference it.

For complete SDS Types documentation and examples, click here.
