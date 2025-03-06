# IO.Swagger.Api.ManagementapplicationsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateAnApplicationV3ManagementApplicationsPost**](ManagementapplicationsApi.md#createanapplicationv3managementapplicationspost) | **POST** /v3/management/applications | Create An Application
[**DeleteAnApplicationV3ManagementApplicationsApplicationIdDelete**](ManagementapplicationsApi.md#deleteanapplicationv3managementapplicationsapplicationiddelete) | **DELETE** /v3/management/applications/{application_id} | Delete An Application
[**GetAnApplicationV3ManagementApplicationsApplicationIdGet**](ManagementapplicationsApi.md#getanapplicationv3managementapplicationsapplicationidget) | **GET** /v3/management/applications/{application_id} | Get An Application
[**ListAllApplicationsV3ManagementApplicationsGet**](ManagementapplicationsApi.md#listallapplicationsv3managementapplicationsget) | **GET** /v3/management/applications | List All Applications
[**UpdateAnApplicationV3ManagementApplicationsApplicationIdPatch**](ManagementapplicationsApi.md#updateanapplicationv3managementapplicationsapplicationidpatch) | **PATCH** /v3/management/applications/{application_id} | Update An Application

<a name="createanapplicationv3managementapplicationspost"></a>
# **CreateAnApplicationV3ManagementApplicationsPost**
> CreateApplicationResponseModel CreateAnApplicationV3ManagementApplicationsPost (CreateApplicationRequestModel body)

Create An Application

Creates an application.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateAnApplicationV3ManagementApplicationsPostExample
    {
        public void main()
        {

            var apiInstance = new ManagementapplicationsApi();
            var body = new CreateApplicationRequestModel(); // CreateApplicationRequestModel | 

            try
            {
                // Create An Application
                CreateApplicationResponseModel result = apiInstance.CreateAnApplicationV3ManagementApplicationsPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementapplicationsApi.CreateAnApplicationV3ManagementApplicationsPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateApplicationRequestModel**](CreateApplicationRequestModel.md)|  | 

### Return type

[**CreateApplicationResponseModel**](CreateApplicationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="deleteanapplicationv3managementapplicationsapplicationiddelete"></a>
# **DeleteAnApplicationV3ManagementApplicationsApplicationIdDelete**
> Object DeleteAnApplicationV3ManagementApplicationsApplicationIdDelete (Object applicationId)

Delete An Application

Deletes the application specified in `application_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class DeleteAnApplicationV3ManagementApplicationsApplicationIdDeleteExample
    {
        public void main()
        {

            var apiInstance = new ManagementapplicationsApi();
            var applicationId = new Object(); // Object | 

            try
            {
                // Delete An Application
                Object result = apiInstance.DeleteAnApplicationV3ManagementApplicationsApplicationIdDelete(applicationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementapplicationsApi.DeleteAnApplicationV3ManagementApplicationsApplicationIdDelete: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **applicationId** | [**Object**](Object.md)|  | 

### Return type

**Object**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="getanapplicationv3managementapplicationsapplicationidget"></a>
# **GetAnApplicationV3ManagementApplicationsApplicationIdGet**
> GetApplicationResponseModel GetAnApplicationV3ManagementApplicationsApplicationIdGet (Object applicationId)

Get An Application

Returns an application matching the provided `application_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetAnApplicationV3ManagementApplicationsApplicationIdGetExample
    {
        public void main()
        {

            var apiInstance = new ManagementapplicationsApi();
            var applicationId = new Object(); // Object | 

            try
            {
                // Get An Application
                GetApplicationResponseModel result = apiInstance.GetAnApplicationV3ManagementApplicationsApplicationIdGet(applicationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementapplicationsApi.GetAnApplicationV3ManagementApplicationsApplicationIdGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **applicationId** | [**Object**](Object.md)|  | 

### Return type

[**GetApplicationResponseModel**](GetApplicationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="listallapplicationsv3managementapplicationsget"></a>
# **ListAllApplicationsV3ManagementApplicationsGet**
> ListApplicationsResponseModel ListAllApplicationsV3ManagementApplicationsGet ()

List All Applications

Lists all applications.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ListAllApplicationsV3ManagementApplicationsGetExample
    {
        public void main()
        {

            var apiInstance = new ManagementapplicationsApi();

            try
            {
                // List All Applications
                ListApplicationsResponseModel result = apiInstance.ListAllApplicationsV3ManagementApplicationsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementapplicationsApi.ListAllApplicationsV3ManagementApplicationsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListApplicationsResponseModel**](ListApplicationsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="updateanapplicationv3managementapplicationsapplicationidpatch"></a>
# **UpdateAnApplicationV3ManagementApplicationsApplicationIdPatch**
> UpdateApplicationResponseModel UpdateAnApplicationV3ManagementApplicationsApplicationIdPatch (UpdateApplicationRequestModel body, Object applicationId)

Update An Application

Updates the application specified in `application_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class UpdateAnApplicationV3ManagementApplicationsApplicationIdPatchExample
    {
        public void main()
        {

            var apiInstance = new ManagementapplicationsApi();
            var body = new UpdateApplicationRequestModel(); // UpdateApplicationRequestModel | 
            var applicationId = new Object(); // Object | 

            try
            {
                // Update An Application
                UpdateApplicationResponseModel result = apiInstance.UpdateAnApplicationV3ManagementApplicationsApplicationIdPatch(body, applicationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementapplicationsApi.UpdateAnApplicationV3ManagementApplicationsApplicationIdPatch: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UpdateApplicationRequestModel**](UpdateApplicationRequestModel.md)|  | 
 **applicationId** | [**Object**](Object.md)|  | 

### Return type

[**UpdateApplicationResponseModel**](UpdateApplicationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
