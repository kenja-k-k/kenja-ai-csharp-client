# IO.Swagger.Api.RagApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateACorpusV3RagCorporaPost**](RagApi.md#createacorpusv3ragcorporapost) | **POST** /v3/rag/corpora | Create A Corpus
[**CreateAReferenceObjectSearchV3RagSearchesReferenceObjectsPost**](RagApi.md#createareferenceobjectsearchv3ragsearchesreferenceobjectspost) | **POST** /v3/rag/searches/reference_objects | Create A Reference Object Search
[**CreatesAReferenceObjectV3RagReferenceObjectsPost**](RagApi.md#createsareferenceobjectv3ragreferenceobjectspost) | **POST** /v3/rag/reference_objects | Creates A Reference Object
[**DeleteACorpusV3RagCorporaCorpusIdDelete**](RagApi.md#deleteacorpusv3ragcorporacorpusiddelete) | **DELETE** /v3/rag/corpora/{corpus_id} | Delete A Corpus
[**DeletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete**](RagApi.md#deletesareferenceobjectv3ragreferenceobjectsreferenceobjectiddelete) | **DELETE** /v3/rag/reference_objects/{reference_object_id} | Deletes A Reference Object
[**GetACorpusV3RagCorporaCorpusIdGet**](RagApi.md#getacorpusv3ragcorporacorpusidget) | **GET** /v3/rag/corpora/{corpus_id} | Get A Corpus
[**GetAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet**](RagApi.md#getareferenceobjectv3ragreferenceobjectsreferenceobjectidget) | **GET** /v3/rag/reference_objects/{reference_object_id} | Get A Reference Object
[**ListAllCorporaV3RagCorporaGet**](RagApi.md#listallcorporav3ragcorporaget) | **GET** /v3/rag/corpora | List All Corpora
[**ListCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet**](RagApi.md#listcorpusreferenceobjectsv3ragcorporacorpusidreferenceobjectsget) | **GET** /v3/rag/corpora/{corpus_id}/reference_objects | List Corpus Reference Objects
[**ListsAllReferenceObjectsV3RagReferenceObjectsGet**](RagApi.md#listsallreferenceobjectsv3ragreferenceobjectsget) | **GET** /v3/rag/reference_objects | Lists All Reference Objects
[**UpdateACorpusV3RagCorporaCorpusIdPatch**](RagApi.md#updateacorpusv3ragcorporacorpusidpatch) | **PATCH** /v3/rag/corpora/{corpus_id} | Update A Corpus

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

            var apiInstance = new RagApi();
            var body = new CreateCorpusRequestModel(); // CreateCorpusRequestModel | 

            try
            {
                // Create A Corpus
                CreateCorpusResponseModel result = apiInstance.CreateACorpusV3RagCorporaPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagApi.CreateACorpusV3RagCorporaPost: " + e.Message );
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

            var apiInstance = new RagApi();
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
                Debug.Print("Exception when calling RagApi.CreateAReferenceObjectSearchV3RagSearchesReferenceObjectsPost: " + e.Message );
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
<a name="createsareferenceobjectv3ragreferenceobjectspost"></a>
# **CreatesAReferenceObjectV3RagReferenceObjectsPost**
> CreateReferenceObjectResponseModel CreatesAReferenceObjectV3RagReferenceObjectsPost (Object uploadFile, Object corpusId)

Creates A Reference Object

Creates an reference object.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreatesAReferenceObjectV3RagReferenceObjectsPostExample
    {
        public void main()
        {

            var apiInstance = new RagApi();
            var uploadFile = new Object(); // Object | 
            var corpusId = new Object(); // Object | 

            try
            {
                // Creates A Reference Object
                CreateReferenceObjectResponseModel result = apiInstance.CreatesAReferenceObjectV3RagReferenceObjectsPost(uploadFile, corpusId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagApi.CreatesAReferenceObjectV3RagReferenceObjectsPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uploadFile** | [**Object**](Object.md)|  | 
 **corpusId** | [**Object**](Object.md)|  | 

### Return type

[**CreateReferenceObjectResponseModel**](CreateReferenceObjectResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: multipart/form-data
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

            var apiInstance = new RagApi();
            var corpusId = new Object(); // Object | 

            try
            {
                // Delete A Corpus
                Object result = apiInstance.DeleteACorpusV3RagCorporaCorpusIdDelete(corpusId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagApi.DeleteACorpusV3RagCorporaCorpusIdDelete: " + e.Message );
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
<a name="deletesareferenceobjectv3ragreferenceobjectsreferenceobjectiddelete"></a>
# **DeletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete**
> Object DeletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete (Object referenceObjectId)

Deletes A Reference Object

Deletes the reference object specified in `reference_object_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class DeletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDeleteExample
    {
        public void main()
        {

            var apiInstance = new RagApi();
            var referenceObjectId = new Object(); // Object | 

            try
            {
                // Deletes A Reference Object
                Object result = apiInstance.DeletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete(referenceObjectId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagApi.DeletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **referenceObjectId** | [**Object**](Object.md)|  | 

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

            var apiInstance = new RagApi();
            var corpusId = new Object(); // Object | 

            try
            {
                // Get A Corpus
                GetCorpusResponseModel result = apiInstance.GetACorpusV3RagCorporaCorpusIdGet(corpusId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagApi.GetACorpusV3RagCorporaCorpusIdGet: " + e.Message );
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
<a name="getareferenceobjectv3ragreferenceobjectsreferenceobjectidget"></a>
# **GetAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet**
> GetReferenceObjectResponseModel GetAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet (Object referenceObjectId)

Get A Reference Object

Returns a reference object matching the provided `reference_object_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGetExample
    {
        public void main()
        {

            var apiInstance = new RagApi();
            var referenceObjectId = new Object(); // Object | 

            try
            {
                // Get A Reference Object
                GetReferenceObjectResponseModel result = apiInstance.GetAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet(referenceObjectId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagApi.GetAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **referenceObjectId** | [**Object**](Object.md)|  | 

### Return type

[**GetReferenceObjectResponseModel**](GetReferenceObjectResponseModel.md)

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

            var apiInstance = new RagApi();

            try
            {
                // List All Corpora
                ListCorporaResponseModel result = apiInstance.ListAllCorporaV3RagCorporaGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagApi.ListAllCorporaV3RagCorporaGet: " + e.Message );
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

            var apiInstance = new RagApi();
            var corpusId = new Object(); // Object | 

            try
            {
                // List Corpus Reference Objects
                ListCorpusReferenceObjectsResponseModel result = apiInstance.ListCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet(corpusId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagApi.ListCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet: " + e.Message );
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
<a name="listsallreferenceobjectsv3ragreferenceobjectsget"></a>
# **ListsAllReferenceObjectsV3RagReferenceObjectsGet**
> ListReferenceObjectsResponseModel ListsAllReferenceObjectsV3RagReferenceObjectsGet ()

Lists All Reference Objects

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
    public class ListsAllReferenceObjectsV3RagReferenceObjectsGetExample
    {
        public void main()
        {

            var apiInstance = new RagApi();

            try
            {
                // Lists All Reference Objects
                ListReferenceObjectsResponseModel result = apiInstance.ListsAllReferenceObjectsV3RagReferenceObjectsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagApi.ListsAllReferenceObjectsV3RagReferenceObjectsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListReferenceObjectsResponseModel**](ListReferenceObjectsResponseModel.md)

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

            var apiInstance = new RagApi();
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
                Debug.Print("Exception when calling RagApi.UpdateACorpusV3RagCorporaCorpusIdPatch: " + e.Message );
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
