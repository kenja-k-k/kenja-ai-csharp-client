# IO.Swagger.Api.RagreferenceObjectsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreatesAReferenceObjectV3RagReferenceObjectsPost**](RagreferenceObjectsApi.md#createsareferenceobjectv3ragreferenceobjectspost) | **POST** /v3/rag/reference_objects | Creates A Reference Object
[**DeletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete**](RagreferenceObjectsApi.md#deletesareferenceobjectv3ragreferenceobjectsreferenceobjectiddelete) | **DELETE** /v3/rag/reference_objects/{reference_object_id} | Deletes A Reference Object
[**GetAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet**](RagreferenceObjectsApi.md#getareferenceobjectv3ragreferenceobjectsreferenceobjectidget) | **GET** /v3/rag/reference_objects/{reference_object_id} | Get A Reference Object
[**ListsAllReferenceObjectsV3RagReferenceObjectsGet**](RagreferenceObjectsApi.md#listsallreferenceobjectsv3ragreferenceobjectsget) | **GET** /v3/rag/reference_objects | Lists All Reference Objects

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

            var apiInstance = new RagreferenceObjectsApi();
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
                Debug.Print("Exception when calling RagreferenceObjectsApi.CreatesAReferenceObjectV3RagReferenceObjectsPost: " + e.Message );
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

            var apiInstance = new RagreferenceObjectsApi();
            var referenceObjectId = new Object(); // Object | 

            try
            {
                // Deletes A Reference Object
                Object result = apiInstance.DeletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete(referenceObjectId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagreferenceObjectsApi.DeletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete: " + e.Message );
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

            var apiInstance = new RagreferenceObjectsApi();
            var referenceObjectId = new Object(); // Object | 

            try
            {
                // Get A Reference Object
                GetReferenceObjectResponseModel result = apiInstance.GetAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet(referenceObjectId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagreferenceObjectsApi.GetAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet: " + e.Message );
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

            var apiInstance = new RagreferenceObjectsApi();

            try
            {
                // Lists All Reference Objects
                ListReferenceObjectsResponseModel result = apiInstance.ListsAllReferenceObjectsV3RagReferenceObjectsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling RagreferenceObjectsApi.ListsAllReferenceObjectsV3RagReferenceObjectsGet: " + e.Message );
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
