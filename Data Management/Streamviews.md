---
uid: Streamviews
---

# Stream views

Stream views provide flexibility in the use of types. While you cannot actually change stream types themselves after you\'ve created them, the stream views feature enables you to create a view of a selected stream that appears as if you had changed the type on which it\'s based.

Types themselves never actually change; the \"changing\" of a type is described in a stream view. You create a stream view by choosing a source and target type as well as a set of mappings between properties of those two types. Using a stream view to leverage existing type properties is preferable to creating an actual new custom type, because the affected stream continues with its previously archived stream data
intact.

You can view either the impact of the stream view on a stream in an ad hoc manner, using a GET call, or you can assign the stream view to a stream in a PUT call.

To view the impact of the stream view on a stream, you can apply a stream view to any read or GET operation. See [API Calls for Reading Data](https://ocs-docs.osisoft.com/Content_Portal/Documentation/SequentialDataStore/Reading_Data_API.html) for examples.

To assign the stream view to a stream, execute an [Update Stream Type](https://ocs-docs.osisoft.com/Content_Portal/Documentation/SequentialDataStore/SDS_Streams.html#update-stream-type) call. By specifying the stream view id in the call, you can effectively assign the target type of the stream view to a specified stream.

**Training Video:** [OCS Portal - What is a Stream View?](https://youtu.be/8iTgWyvc7eQ)

**Training Video:** [Create a Stream View in the OCS Portal](https://youtu.be/jhLqmLN0rQE)

For more information, see [Stream Views](https://ocs-docs.osisoft.com/Content_Portal/Documentation/SequentialDataStore/SDS_Views.html) in OCS Docs.

## Search

Type the name of any known stream view in the **Search** window to
retrieve an existing stream view.

* To create a new stream view, click **Stream views** in the **Storage Explorer** pane, and then click **Add Stream View**.

* To edit a stream view, select an existing stream view, and then click **Edit Stream View**.

* To delete a stream view, select an existing stream view, or hold down the **Ctrl** key and select multiple stream views, and then click **Remove Stream View**.