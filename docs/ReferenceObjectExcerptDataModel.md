# IO.Swagger.Model.ReferenceObjectExcerptDataModel
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ReferenceObjectId** | **Object** | The UUID of the original reference object. | 
**PageNum** | **Object** | The page number this excerpt is found at, indexed from 0. Value of -1 means pages are not supported.         This is much less useful than the actual chunk index, but users are dumb so what can you do really... | [optional] [default to 0]
**Offset** | **Object** | The offset at which this excerpt starts. | [optional] [default to 0]
**SourceId** | **Object** | The original source ID for this reference object. This field is not used internally, you can set it to any value you want. | [optional] 
**SourceName** | **Object** | The original source name for this reference object. | [optional] 
**SourceUrl** | **Object** | The original source URL for this reference object - if any. | [optional] 
**ObjectType** | **ReferenceObjectType** | The type of this reference object. | [optional] [default to ReferenceObjectType.File]
**Content** | **Object** | The content of the reference object excerpt. | [optional] 
**Score** | **Object** | The relevance score. | [optional] [default to 0]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

