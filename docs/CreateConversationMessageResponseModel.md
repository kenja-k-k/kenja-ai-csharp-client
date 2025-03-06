# IO.Swagger.Model.CreateConversationMessageResponseModel
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Question** | [**ConversationMessageDataModel**](ConversationMessageDataModel.md) | The question (message) created by the user. | 
**Response** | [**ConversationMessageDataModel**](ConversationMessageDataModel.md) | The response from the LLM. | 
**ReferenceObjectExcerpts** | **Object** |  | [optional] [default to []]
**QueryPipelineId** | **QueryPipelineID** | Used query pipeline. | 
**LlmInferenceProviderId** | **LLMInferenceProviderID** | Used LLM inference provider. | 
**LlmModelId** | **LLMModelID** | Used LLM inference provider. | 
**UsageInfo** | [**UsageInfoModel**](UsageInfoModel.md) | Request usage information. | 
**PipelineTrace** | **Object** | Pipeline trace. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

