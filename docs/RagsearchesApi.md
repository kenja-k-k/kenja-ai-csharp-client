# IO.Swagger.Api.RagsearchesApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateAReferenceObjectSearchV3RagSearchesReferenceObjectsPost**](RagsearchesApi.md#createareferenceobjectsearchv3ragsearchesreferenceobjectspost) | **POST** /v3/rag/searches/reference_objects | Create A Reference Object Search

<a name="createareferenceobjectsearchv3ragsearchesreferenceobjectspost"></a>
# **CreateAReferenceObjectSearchV3RagSearchesReferenceObjectsPost**
> CreateReferenceObjectSearchResponseModel CreateAReferenceObjectSearchV3RagSearchesReferenceObjectsPost (CreateReferenceObjectSearchRequestModel body, Object corpusId = null)

Create A Reference Object Search

Creates a reference object search query and returns results.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateAReferenceObjectSearchV3RagSearchesReferenceObjectsPostExample
    {
        public void main()
        {

            var apiInstance = new RagsearchesApi();
            var body = new CreateReferenceObjectSearchRequestModel(); // CreateReferenceObjectSearchRequestModel | 
            var corpusId = new Object(); // Object |  (optional) 

            try
            {
                // Create A Reference Object Search
                CreateReferenceObjectSearchResponseModel result = apiInstance.CreateAReferenceObjectSearchV3RagSearchesReferenceObjectsPost(body, corpusId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagsearchesApi.CreateAReferenceObjectSearchV3RagSearchesReferenceObjectsPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateReferenceObjectSearchRequestModel**](CreateReferenceObjectSearchRequestModel.md)|  | 
 **corpusId** | [**Object**](Object.md)|  | [optional] 

### Return type

[**CreateReferenceObjectSearchResponseModel**](CreateReferenceObjectSearchResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
