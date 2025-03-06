# IO.Swagger.Api.ModelsllmsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost**](ModelsllmsApi.md#createacompletionv3modelsllminferenceprovidersllminferenceprovideridllmsllmmodelidpost) | **POST** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id} | Create A Completion
[**CreateAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost**](ModelsllmsApi.md#createastreamingcompletionv3modelsllminferenceprovidersllminferenceprovideridllmsllmmodelidstreampost) | **POST** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id}/stream | Create A Streaming Completion
[**GetModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet**](ModelsllmsApi.md#getmodelinformationv3modelsllminferenceprovidersllminferenceprovideridllmsllmmodelidget) | **GET** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id} | Get Model Information
[**ListAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet**](ModelsllmsApi.md#listallllminferenceprovidersv3modelsllminferenceprovidersget) | **GET** /v3/models/llm_inference_providers | List All Llm Inference Providers
[**ListLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet**](ModelsllmsApi.md#listllminferenceprovidermodelsv3modelsllminferenceprovidersllminferenceprovideridllmsget) | **GET** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms | List Llm Inference Provider Models

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

            var apiInstance = new ModelsllmsApi();
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
                Debug.Print("Exception when calling ModelsllmsApi.CreateACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost: " + e.Message );
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

            var apiInstance = new ModelsllmsApi();
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
                Debug.Print("Exception when calling ModelsllmsApi.CreateAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost: " + e.Message );
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

            var apiInstance = new ModelsllmsApi();
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
                Debug.Print("Exception when calling ModelsllmsApi.GetModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet: " + e.Message );
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

            var apiInstance = new ModelsllmsApi();

            try
            {
                // List All Llm Inference Providers
                ListLLMInferenceProvidersResponseModel result = apiInstance.ListAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ModelsllmsApi.ListAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet: " + e.Message );
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

            var apiInstance = new ModelsllmsApi();
            var llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 

            try
            {
                // List Llm Inference Provider Models
                ListLLMInferenceProviderModelsResponseModel result = apiInstance.ListLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet(llmInferenceProviderId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ModelsllmsApi.ListLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet: " + e.Message );
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
