# IO.Swagger.Model.ReferenceObjectDataModel
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **Object** | The UUID of this reference object. | [optional] 
**ApplicationId** | **Object** | The UUID of the application associated with this reference object. | 
**CorpusId** | **Object** | The UUID of the corpus associated with this reference object. | 
**SourceId** | **Object** | The original source ID for this reference object. This field is not used internally, you can set it to any value you want. | [optional] 
**SourceName** | **Object** | The original source name for this reference object. | [optional] 
**SourceUrl** | **Object** | The original source URL for this reference object - if any. | [optional] 
**Size** | **Object** | The size of this reference object (in bytes). | [optional] [default to 0]
**Hash** | **Object** | The hash of this reference object. This value is generated automatically, if you set it - it will be ignored. | [optional] 
**Status** | **ReferenceObjectStatus** | The status of this reference object. | [optional] [default to ReferenceObjectStatus.Queued]
**EmbeddingIds** | **Object** | Embedding IDs associated with this reference object. | [optional] [default to []]
**ObjectType** | **ReferenceObjectType** | The type of this reference object. | [optional] [default to ReferenceObjectType.File]
**Content** | **Object** | The content of the reference object (enumerated by page). | [optional] 
**Summary** | **Object** | The summary of the reference object created by an LLM. | [optional] 
**CreatedAt** | **Object** | Creation date of this reference object. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

