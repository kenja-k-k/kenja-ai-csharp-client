# IO.Swagger.Model.ConversationMessageDataModel
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **Object** | The UUID of this conversation message. | [optional] 
**ApplicationId** | **Object** | The UUID of the application associated with this conversation message. | 
**ConversationId** | **Object** | The UUID of the conversation associated with this conversation message. | 
**CorpusId** | **Object** | The UUID of the corpus associated with this conversation message. | [optional] 
**Origin** | **ConversationMessageOrigin** | The origin of this conversation message. | 
**Content** | **Object** | The content of this conversation message. | 
**ResponseToConversationMessageId** | **Object** | The UUID of the conversation message this one is a response to. | [optional] 
**NonHallucinationScore** | **Object** | How non-hallucinatory the answer is. | [optional] [default to 0]
**FactualityScore** | **Object** | How factual the answer is. | [optional] [default to 0]
**LlmInferenceProviderId** | **Object** | The LLM inference provider associated with this message. | [optional] 
**LlmModelId** | **Object** | The LLM model associated with this message. | [optional] 
**ReferenceObjectIds** | **Object** | Reference object UUIDs associated with this conversation message. | [optional] [default to []]
**CreatedAt** | **Object** | The creation date of this conversation message. | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

