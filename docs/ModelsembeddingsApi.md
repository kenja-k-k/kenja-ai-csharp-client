# IO.Swagger.Api.ModelsembeddingsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ListAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet**](ModelsembeddingsApi.md#listallembeddinginferenceprovidersv3modelsembeddingsget) | **GET** /v3/models/embeddings | List All Embedding Inference Providers
[**ListEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet**](ModelsembeddingsApi.md#listembeddinginferenceprovidermodelsv3modelsembeddingsembeddinginferenceprovideridget) | **GET** /v3/models/embeddings/{embedding_inference_provider_id} | List Embedding Inference Provider Models

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

            var apiInstance = new ModelsembeddingsApi();

            try
            {
                // List All Embedding Inference Providers
                ListEmbeddingInferenceProvidersResponseModel result = apiInstance.ListAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ModelsembeddingsApi.ListAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet: " + e.Message );
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

            var apiInstance = new ModelsembeddingsApi();
            var embeddingInferenceProviderId = new EmbeddingInferenceProviderID(); // EmbeddingInferenceProviderID | 

            try
            {
                // List Embedding Inference Provider Models
                ListEmbeddingInferenceProviderModelsResponseModel result = apiInstance.ListEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet(embeddingInferenceProviderId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ModelsembeddingsApi.ListEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet: " + e.Message );
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
