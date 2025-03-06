# IO.Swagger.Api.ManagementApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateAnApplicationV3ManagementApplicationsPost**](ManagementApi.md#createanapplicationv3managementapplicationspost) | **POST** /v3/management/applications | Create An Application
[**CreateAnOrganizationV3ManagementOrganizationsPost**](ManagementApi.md#createanorganizationv3managementorganizationspost) | **POST** /v3/management/organizations | Create An Organization
[**DeleteAnApplicationV3ManagementApplicationsApplicationIdDelete**](ManagementApi.md#deleteanapplicationv3managementapplicationsapplicationiddelete) | **DELETE** /v3/management/applications/{application_id} | Delete An Application
[**DeleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete**](ManagementApi.md#deleteanorganizationv3managementorganizationsorganizationiddelete) | **DELETE** /v3/management/organizations/{organization_id} | Delete An Organization
[**GetAnApplicationV3ManagementApplicationsApplicationIdGet**](ManagementApi.md#getanapplicationv3managementapplicationsapplicationidget) | **GET** /v3/management/applications/{application_id} | Get An Application
[**GetAnOrganizationV3ManagementOrganizationsOrganizationIdGet**](ManagementApi.md#getanorganizationv3managementorganizationsorganizationidget) | **GET** /v3/management/organizations/{organization_id} | Get An Organization
[**ListAllApplicationsV3ManagementApplicationsGet**](ManagementApi.md#listallapplicationsv3managementapplicationsget) | **GET** /v3/management/applications | List All Applications
[**ListAllOrganizationsV3ManagementOrganizationsGet**](ManagementApi.md#listallorganizationsv3managementorganizationsget) | **GET** /v3/management/organizations | List All Organizations
[**ListOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet**](ManagementApi.md#listorganizationapplicationsv3managementorganizationsorganizationidapplicationsget) | **GET** /v3/management/organizations/{organization_id}/applications | List Organization Applications
[**UpdateAnApplicationV3ManagementApplicationsApplicationIdPatch**](ManagementApi.md#updateanapplicationv3managementapplicationsapplicationidpatch) | **PATCH** /v3/management/applications/{application_id} | Update An Application
[**UpdateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch**](ManagementApi.md#updateanorganizationv3managementorganizationsorganizationidpatch) | **PATCH** /v3/management/organizations/{organization_id} | Update An Organization

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

            var apiInstance = new ManagementApi();
            var body = new CreateApplicationRequestModel(); // CreateApplicationRequestModel | 

            try
            {
                // Create An Application
                CreateApplicationResponseModel result = apiInstance.CreateAnApplicationV3ManagementApplicationsPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementApi.CreateAnApplicationV3ManagementApplicationsPost: " + e.Message );
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
<a name="createanorganizationv3managementorganizationspost"></a>
# **CreateAnOrganizationV3ManagementOrganizationsPost**
> CreateOrganizationResponseModel CreateAnOrganizationV3ManagementOrganizationsPost (CreateOrganizationRequestModel body)

Create An Organization

Creates an organization.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateAnOrganizationV3ManagementOrganizationsPostExample
    {
        public void main()
        {

            var apiInstance = new ManagementApi();
            var body = new CreateOrganizationRequestModel(); // CreateOrganizationRequestModel | 

            try
            {
                // Create An Organization
                CreateOrganizationResponseModel result = apiInstance.CreateAnOrganizationV3ManagementOrganizationsPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementApi.CreateAnOrganizationV3ManagementOrganizationsPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateOrganizationRequestModel**](CreateOrganizationRequestModel.md)|  | 

### Return type

[**CreateOrganizationResponseModel**](CreateOrganizationResponseModel.md)

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

            var apiInstance = new ManagementApi();
            var applicationId = new Object(); // Object | 

            try
            {
                // Delete An Application
                Object result = apiInstance.DeleteAnApplicationV3ManagementApplicationsApplicationIdDelete(applicationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementApi.DeleteAnApplicationV3ManagementApplicationsApplicationIdDelete: " + e.Message );
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
<a name="deleteanorganizationv3managementorganizationsorganizationiddelete"></a>
# **DeleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete**
> Object DeleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete (Object organizationId)

Delete An Organization

Deletes the organization specified in `organization_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class DeleteAnOrganizationV3ManagementOrganizationsOrganizationIdDeleteExample
    {
        public void main()
        {

            var apiInstance = new ManagementApi();
            var organizationId = new Object(); // Object | 

            try
            {
                // Delete An Organization
                Object result = apiInstance.DeleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete(organizationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementApi.DeleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organizationId** | [**Object**](Object.md)|  | 

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

            var apiInstance = new ManagementApi();
            var applicationId = new Object(); // Object | 

            try
            {
                // Get An Application
                GetApplicationResponseModel result = apiInstance.GetAnApplicationV3ManagementApplicationsApplicationIdGet(applicationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementApi.GetAnApplicationV3ManagementApplicationsApplicationIdGet: " + e.Message );
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
<a name="getanorganizationv3managementorganizationsorganizationidget"></a>
# **GetAnOrganizationV3ManagementOrganizationsOrganizationIdGet**
> GetOrganizationResponseModel GetAnOrganizationV3ManagementOrganizationsOrganizationIdGet (Object organizationId)

Get An Organization

Returns an organization matching the provided `organization_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetAnOrganizationV3ManagementOrganizationsOrganizationIdGetExample
    {
        public void main()
        {

            var apiInstance = new ManagementApi();
            var organizationId = new Object(); // Object | 

            try
            {
                // Get An Organization
                GetOrganizationResponseModel result = apiInstance.GetAnOrganizationV3ManagementOrganizationsOrganizationIdGet(organizationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementApi.GetAnOrganizationV3ManagementOrganizationsOrganizationIdGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organizationId** | [**Object**](Object.md)|  | 

### Return type

[**GetOrganizationResponseModel**](GetOrganizationResponseModel.md)

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

            var apiInstance = new ManagementApi();

            try
            {
                // List All Applications
                ListApplicationsResponseModel result = apiInstance.ListAllApplicationsV3ManagementApplicationsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementApi.ListAllApplicationsV3ManagementApplicationsGet: " + e.Message );
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
<a name="listallorganizationsv3managementorganizationsget"></a>
# **ListAllOrganizationsV3ManagementOrganizationsGet**
> ListOrganizationsResponseModel ListAllOrganizationsV3ManagementOrganizationsGet ()

List All Organizations

Lists all organizations.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ListAllOrganizationsV3ManagementOrganizationsGetExample
    {
        public void main()
        {

            var apiInstance = new ManagementApi();

            try
            {
                // List All Organizations
                ListOrganizationsResponseModel result = apiInstance.ListAllOrganizationsV3ManagementOrganizationsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementApi.ListAllOrganizationsV3ManagementOrganizationsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListOrganizationsResponseModel**](ListOrganizationsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="listorganizationapplicationsv3managementorganizationsorganizationidapplicationsget"></a>
# **ListOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet**
> ListOrganizationApplicationsResponseModel ListOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet (Object organizationId)

List Organization Applications

Lists all applications associated with an organization specified in `organization_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ListOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGetExample
    {
        public void main()
        {

            var apiInstance = new ManagementApi();
            var organizationId = new Object(); // Object | 

            try
            {
                // List Organization Applications
                ListOrganizationApplicationsResponseModel result = apiInstance.ListOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet(organizationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementApi.ListOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organizationId** | [**Object**](Object.md)|  | 

### Return type

[**ListOrganizationApplicationsResponseModel**](ListOrganizationApplicationsResponseModel.md)

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

            var apiInstance = new ManagementApi();
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
                Debug.Print("Exception when calling ManagementApi.UpdateAnApplicationV3ManagementApplicationsApplicationIdPatch: " + e.Message );
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
<a name="updateanorganizationv3managementorganizationsorganizationidpatch"></a>
# **UpdateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch**
> UpdateOrganizationResponseModel UpdateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch (UpdateOrganizationRequestModel body, Object organizationId)

Update An Organization

Updates the organization specified in `organization_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class UpdateAnOrganizationV3ManagementOrganizationsOrganizationIdPatchExample
    {
        public void main()
        {

            var apiInstance = new ManagementApi();
            var body = new UpdateOrganizationRequestModel(); // UpdateOrganizationRequestModel | 
            var organizationId = new Object(); // Object | 

            try
            {
                // Update An Organization
                UpdateOrganizationResponseModel result = apiInstance.UpdateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch(body, organizationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementApi.UpdateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UpdateOrganizationRequestModel**](UpdateOrganizationRequestModel.md)|  | 
 **organizationId** | [**Object**](Object.md)|  | 

### Return type

[**UpdateOrganizationResponseModel**](UpdateOrganizationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
