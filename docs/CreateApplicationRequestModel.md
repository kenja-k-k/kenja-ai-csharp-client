# IO.Swagger.Model.CreateApplicationRequestModel
## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | **Object** | The name of this application. | 
**OrganizationId** | **Object** | The UUID of the organization behind this application. | 
**ApiCallsLimitPerMonth** | **Object** | The maximum amount of API calls this application can make in a month. | [optional] [default to 0]
**LlmTokensLimitPerMonth** | **Object** | The maximum amount of LLM tokens (combined I/O) this application can use in a month. | [optional] [default to 0]
**EmbeddingTokensLimitPerMonth** | **Object** | The maximum amount of embedding tokens this application can use in a month. | [optional] [default to 0]
**ImageGenerationLimitPerMonth** | **Object** | The maximum amount of images this application can generate in a month. | [optional] [default to 0]
**AllowLlmQueries** | **Object** | Should this application be allowed to make queries to LLMs? | [optional] [default to true]
**AllowCorpusCreation** | **Object** | Should this application be allowed to create corpuses? | [optional] [default to true]
**AllowImageGeneration** | **Object** | Should this application be allowed to create images? | [optional] [default to true]
**AllowExpensiveQueries** | **Object** | Should this application be allowed to make potentially expensive queries? | [optional] [default to true]
**WebhookUrl** | **Object** | Webhook URL to use when notifying of queued events. | [optional] 
**IsActive** | **Object** | Is this application active? | [optional] [default to true]

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)

