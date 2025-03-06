# IO.Swagger.Model.CreateConversationMessageRequestModel
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Content** | **Object** | Semantic/keyword based prompt. | 
**CorpusId** | **Object** | The corpus to query. | [optional] 
**IncludeReferenceObjects** | **Object** | Explicitly include specified reference objects when searching.                     Setting this will limit search only to reference objects specified here. | [optional] [default to []]
**FactualityMode** | **Object** | The factuality mode requested. | [optional] [default to grounded]
**Temperature** | **Object** | LLM model temperature. | [optional] [default to 0.8]
**WithPipelineTrace** | **Object** | Include the pipeline trace. | [optional] [default to false]
**LlmInferenceProviderId** | **Object** | The LLM inference provider to use. | [optional] [default to vertex-ai]
**LlmModelId** | **Object** | The LLM model to use. | [optional] [default to vertex-ai.gemini-2.0-pro]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

