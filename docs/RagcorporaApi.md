# IO.Swagger.Api.RagcorporaApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateACorpusV3RagCorporaPost**](RagcorporaApi.md#createacorpusv3ragcorporapost) | **POST** /v3/rag/corpora | Create A Corpus
[**DeleteACorpusV3RagCorporaCorpusIdDelete**](RagcorporaApi.md#deleteacorpusv3ragcorporacorpusiddelete) | **DELETE** /v3/rag/corpora/{corpus_id} | Delete A Corpus
[**GetACorpusV3RagCorporaCorpusIdGet**](RagcorporaApi.md#getacorpusv3ragcorporacorpusidget) | **GET** /v3/rag/corpora/{corpus_id} | Get A Corpus
[**ListAllCorporaV3RagCorporaGet**](RagcorporaApi.md#listallcorporav3ragcorporaget) | **GET** /v3/rag/corpora | List All Corpora
[**ListCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet**](RagcorporaApi.md#listcorpusreferenceobjectsv3ragcorporacorpusidreferenceobjectsget) | **GET** /v3/rag/corpora/{corpus_id}/reference_objects | List Corpus Reference Objects
[**UpdateACorpusV3RagCorporaCorpusIdPatch**](RagcorporaApi.md#updateacorpusv3ragcorporacorpusidpatch) | **PATCH** /v3/rag/corpora/{corpus_id} | Update A Corpus

<a name="createacorpusv3ragcorporapost"></a>
# **CreateACorpusV3RagCorporaPost**
> CreateCorpusResponseModel CreateACorpusV3RagCorporaPost (CreateCorpusRequestModel body)

Create A Corpus

Creates a corpus.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateACorpusV3RagCorporaPostExample
    {
        public void main()
        {

            var apiInstance = new RagcorporaApi();
            var body = new CreateCorpusRequestModel(); // CreateCorpusRequestModel | 

            try
            {
                // Create A Corpus
                CreateCorpusResponseModel result = apiInstance.CreateACorpusV3RagCorporaPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagcorporaApi.CreateACorpusV3RagCorporaPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateCorpusRequestModel**](CreateCorpusRequestModel.md)|  | 

### Return type

[**CreateCorpusResponseModel**](CreateCorpusResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="deleteacorpusv3ragcorporacorpusiddelete"></a>
# **DeleteACorpusV3RagCorporaCorpusIdDelete**
> Object DeleteACorpusV3RagCorporaCorpusIdDelete (Object corpusId)

Delete A Corpus

Deletes the corpus specified in `corpus_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class DeleteACorpusV3RagCorporaCorpusIdDeleteExample
    {
        public void main()
        {

            var apiInstance = new RagcorporaApi();
            var corpusId = new Object(); // Object | 

            try
            {
                // Delete A Corpus
                Object result = apiInstance.DeleteACorpusV3RagCorporaCorpusIdDelete(corpusId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagcorporaApi.DeleteACorpusV3RagCorporaCorpusIdDelete: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **corpusId** | [**Object**](Object.md)|  | 

### Return type

**Object**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="getacorpusv3ragcorporacorpusidget"></a>
# **GetACorpusV3RagCorporaCorpusIdGet**
> GetCorpusResponseModel GetACorpusV3RagCorporaCorpusIdGet (Object corpusId)

Get A Corpus

Returns a corpus matching the provided `corpus_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetACorpusV3RagCorporaCorpusIdGetExample
    {
        public void main()
        {

            var apiInstance = new RagcorporaApi();
            var corpusId = new Object(); // Object | 

            try
            {
                // Get A Corpus
                GetCorpusResponseModel result = apiInstance.GetACorpusV3RagCorporaCorpusIdGet(corpusId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagcorporaApi.GetACorpusV3RagCorporaCorpusIdGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **corpusId** | [**Object**](Object.md)|  | 

### Return type

[**GetCorpusResponseModel**](GetCorpusResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="listallcorporav3ragcorporaget"></a>
# **ListAllCorporaV3RagCorporaGet**
> ListCorporaResponseModel ListAllCorporaV3RagCorporaGet ()

List All Corpora

Lists all corpora.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ListAllCorporaV3RagCorporaGetExample
    {
        public void main()
        {

            var apiInstance = new RagcorporaApi();

            try
            {
                // List All Corpora
                ListCorporaResponseModel result = apiInstance.ListAllCorporaV3RagCorporaGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagcorporaApi.ListAllCorporaV3RagCorporaGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListCorporaResponseModel**](ListCorporaResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="listcorpusreferenceobjectsv3ragcorporacorpusidreferenceobjectsget"></a>
# **ListCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet**
> ListCorpusReferenceObjectsResponseModel ListCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet (Object corpusId)

List Corpus Reference Objects

Lists all reference objects associated with a corpus specified in `organization_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ListCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGetExample
    {
        public void main()
        {

            var apiInstance = new RagcorporaApi();
            var corpusId = new Object(); // Object | 

            try
            {
                // List Corpus Reference Objects
                ListCorpusReferenceObjectsResponseModel result = apiInstance.ListCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet(corpusId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagcorporaApi.ListCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **corpusId** | [**Object**](Object.md)|  | 

### Return type

[**ListCorpusReferenceObjectsResponseModel**](ListCorpusReferenceObjectsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="updateacorpusv3ragcorporacorpusidpatch"></a>
# **UpdateACorpusV3RagCorporaCorpusIdPatch**
> UpdateCorpusResponseModel UpdateACorpusV3RagCorporaCorpusIdPatch (UpdateCorpusRequestModel body, Object corpusId)

Update A Corpus

Updates the corpus specified in `corpus_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class UpdateACorpusV3RagCorporaCorpusIdPatchExample
    {
        public void main()
        {

            var apiInstance = new RagcorporaApi();
            var body = new UpdateCorpusRequestModel(); // UpdateCorpusRequestModel | 
            var corpusId = new Object(); // Object | 

            try
            {
                // Update A Corpus
                UpdateCorpusResponseModel result = apiInstance.UpdateACorpusV3RagCorporaCorpusIdPatch(body, corpusId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagcorporaApi.UpdateACorpusV3RagCorporaCorpusIdPatch: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UpdateCorpusRequestModel**](UpdateCorpusRequestModel.md)|  | 
 **corpusId** | [**Object**](Object.md)|  | 

### Return type

[**UpdateCorpusResponseModel**](UpdateCorpusResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
