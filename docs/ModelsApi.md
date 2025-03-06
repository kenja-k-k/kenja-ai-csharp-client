# IO.Swagger.Api.ModelsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost**](ModelsApi.md#createacompletionv3modelsllminferenceprovidersllminferenceprovideridllmsllmmodelidpost) | **POST** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id} | Create A Completion
[**CreateAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost**](ModelsApi.md#createastreamingcompletionv3modelsllminferenceprovidersllminferenceprovideridllmsllmmodelidstreampost) | **POST** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id}/stream | Create A Streaming Completion
[**GetModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet**](ModelsApi.md#getmodelinformationv3modelsllminferenceprovidersllminferenceprovideridllmsllmmodelidget) | **GET** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id} | Get Model Information
[**ListAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet**](ModelsApi.md#listallembeddinginferenceprovidersv3modelsembeddingsget) | **GET** /v3/models/embeddings | List All Embedding Inference Providers
[**ListAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet**](ModelsApi.md#listallllminferenceprovidersv3modelsllminferenceprovidersget) | **GET** /v3/models/llm_inference_providers | List All Llm Inference Providers
[**ListEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet**](ModelsApi.md#listembeddinginferenceprovidermodelsv3modelsembeddingsembeddinginferenceprovideridget) | **GET** /v3/models/embeddings/{embedding_inference_provider_id} | List Embedding Inference Provider Models
[**ListLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet**](ModelsApi.md#listllminferenceprovidermodelsv3modelsllminferenceprovidersllminferenceprovideridllmsget) | **GET** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms | List Llm Inference Provider Models

<a name="createacompletionv3modelsllminferenceprovidersllminferenceprovideridllmsllmmodelidpost"></a>
# **CreateACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost**
> CreateLLMCompletionResponseModel CreateACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost (CreateLLMCompletionRequestModel body, LLMInferenceProviderID llmInferenceProviderId, LLMModelID llmModelId)

Create A Completion

Creates an LLM completion.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPostExample
    {
        public void main()
        {

            var apiInstance = new ModelsApi();
            var body = new CreateLLMCompletionRequestModel(); // CreateLLMCompletionRequestModel | 
            var llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 
            var llmModelId = new LLMModelID(); // LLMModelID | 

            try
            {
                // Create A Completion
                CreateLLMCompletionResponseModel result = apiInstance.CreateACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost(body, llmInferenceProviderId, llmModelId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ModelsApi.CreateACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateLLMCompletionRequestModel**](CreateLLMCompletionRequestModel.md)|  | 
 **llmInferenceProviderId** | [**LLMInferenceProviderID**](LLMInferenceProviderID.md)|  | 
 **llmModelId** | [**LLMModelID**](LLMModelID.md)|  | 

### Return type

[**CreateLLMCompletionResponseModel**](CreateLLMCompletionResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="createastreamingcompletionv3modelsllminferenceprovidersllminferenceprovideridllmsllmmodelidstreampost"></a>
# **CreateAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost**
> Object CreateAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost (CreateLLMCompletionRequestModel body, LLMInferenceProviderID llmInferenceProviderId, LLMModelID llmModelId)

Create A Streaming Completion

Creates a streaming LLM completion.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPostExample
    {
        public void main()
        {

            var apiInstance = new ModelsApi();
            var body = new CreateLLMCompletionRequestModel(); // CreateLLMCompletionRequestModel | 
            var llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 
            var llmModelId = new LLMModelID(); // LLMModelID | 

            try
            {
                // Create A Streaming Completion
                Object result = apiInstance.CreateAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost(body, llmInferenceProviderId, llmModelId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ModelsApi.CreateAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateLLMCompletionRequestModel**](CreateLLMCompletionRequestModel.md)|  | 
 **llmInferenceProviderId** | [**LLMInferenceProviderID**](LLMInferenceProviderID.md)|  | 
 **llmModelId** | [**LLMModelID**](LLMModelID.md)|  | 

### Return type

**Object**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="getmodelinformationv3modelsllminferenceprovidersllminferenceprovideridllmsllmmodelidget"></a>
# **GetModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet**
> GetLLMModelResponseModel GetModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet (LLMInferenceProviderID llmInferenceProviderId, LLMModelID llmModelId)

Get Model Information

Gets information for a specified model.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGetExample
    {
        public void main()
        {

            var apiInstance = new ModelsApi();
            var llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 
            var llmModelId = new LLMModelID(); // LLMModelID | 

            try
            {
                // Get Model Information
                GetLLMModelResponseModel result = apiInstance.GetModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet(llmInferenceProviderId, llmModelId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ModelsApi.GetModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **llmInferenceProviderId** | [**LLMInferenceProviderID**](LLMInferenceProviderID.md)|  | 
 **llmModelId** | [**LLMModelID**](LLMModelID.md)|  | 

### Return type

[**GetLLMModelResponseModel**](GetLLMModelResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="listallembeddinginferenceprovidersv3modelsembeddingsget"></a>
# **ListAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet**
> ListEmbeddingInferenceProvidersResponseModel ListAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet ()

List All Embedding Inference Providers

List all embedding inference providers.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ListAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGetExample
    {
        public void main()
        {

            var apiInstance = new ModelsApi();

            try
            {
                // List All Embedding Inference Providers
                ListEmbeddingInferenceProvidersResponseModel result = apiInstance.ListAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ModelsApi.ListAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListEmbeddingInferenceProvidersResponseModel**](ListEmbeddingInferenceProvidersResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="listallllminferenceprovidersv3modelsllminferenceprovidersget"></a>
# **ListAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet**
> ListLLMInferenceProvidersResponseModel ListAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet ()

List All Llm Inference Providers

List all LLM inference providers.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ListAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGetExample
    {
        public void main()
        {

            var apiInstance = new ModelsApi();

            try
            {
                // List All Llm Inference Providers
                ListLLMInferenceProvidersResponseModel result = apiInstance.ListAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ModelsApi.ListAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListLLMInferenceProvidersResponseModel**](ListLLMInferenceProvidersResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="listembeddinginferenceprovidermodelsv3modelsembeddingsembeddinginferenceprovideridget"></a>
# **ListEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet**
> ListEmbeddingInferenceProviderModelsResponseModel ListEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet (EmbeddingInferenceProviderID embeddingInferenceProviderId)

List Embedding Inference Provider Models

Lists all embedding models in the provided embedding inference provider.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ListEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGetExample
    {
        public void main()
        {

            var apiInstance = new ModelsApi();
            var embeddingInferenceProviderId = new EmbeddingInferenceProviderID(); // EmbeddingInferenceProviderID | 

            try
            {
                // List Embedding Inference Provider Models
                ListEmbeddingInferenceProviderModelsResponseModel result = apiInstance.ListEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet(embeddingInferenceProviderId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ModelsApi.ListEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **embeddingInferenceProviderId** | [**EmbeddingInferenceProviderID**](EmbeddingInferenceProviderID.md)|  | 

### Return type

[**ListEmbeddingInferenceProviderModelsResponseModel**](ListEmbeddingInferenceProviderModelsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="listllminferenceprovidermodelsv3modelsllminferenceprovidersllminferenceprovideridllmsget"></a>
# **ListLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet**
> ListLLMInferenceProviderModelsResponseModel ListLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet (LLMInferenceProviderID llmInferenceProviderId)

List Llm Inference Provider Models

Lists all LLM models in the provided llm inference provider.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ListLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGetExample
    {
        public void main()
        {

            var apiInstance = new ModelsApi();
            var llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 

            try
            {
                // List Llm Inference Provider Models
                ListLLMInferenceProviderModelsResponseModel result = apiInstance.ListLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet(llmInferenceProviderId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ModelsApi.ListLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **llmInferenceProviderId** | [**LLMInferenceProviderID**](LLMInferenceProviderID.md)|  | 

### Return type

[**ListLLMInferenceProviderModelsResponseModel**](ListLLMInferenceProviderModelsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
