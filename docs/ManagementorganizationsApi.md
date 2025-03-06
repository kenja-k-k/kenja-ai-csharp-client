# IO.Swagger.Api.ManagementorganizationsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateAnOrganizationV3ManagementOrganizationsPost**](ManagementorganizationsApi.md#createanorganizationv3managementorganizationspost) | **POST** /v3/management/organizations | Create An Organization
[**DeleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete**](ManagementorganizationsApi.md#deleteanorganizationv3managementorganizationsorganizationiddelete) | **DELETE** /v3/management/organizations/{organization_id} | Delete An Organization
[**GetAnOrganizationV3ManagementOrganizationsOrganizationIdGet**](ManagementorganizationsApi.md#getanorganizationv3managementorganizationsorganizationidget) | **GET** /v3/management/organizations/{organization_id} | Get An Organization
[**ListAllOrganizationsV3ManagementOrganizationsGet**](ManagementorganizationsApi.md#listallorganizationsv3managementorganizationsget) | **GET** /v3/management/organizations | List All Organizations
[**ListOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet**](ManagementorganizationsApi.md#listorganizationapplicationsv3managementorganizationsorganizationidapplicationsget) | **GET** /v3/management/organizations/{organization_id}/applications | List Organization Applications
[**UpdateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch**](ManagementorganizationsApi.md#updateanorganizationv3managementorganizationsorganizationidpatch) | **PATCH** /v3/management/organizations/{organization_id} | Update An Organization

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

            var apiInstance = new ManagementorganizationsApi();
            var body = new CreateOrganizationRequestModel(); // CreateOrganizationRequestModel | 

            try
            {
                // Create An Organization
                CreateOrganizationResponseModel result = apiInstance.CreateAnOrganizationV3ManagementOrganizationsPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementorganizationsApi.CreateAnOrganizationV3ManagementOrganizationsPost: " + e.Message );
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

            var apiInstance = new ManagementorganizationsApi();
            var organizationId = new Object(); // Object | 

            try
            {
                // Delete An Organization
                Object result = apiInstance.DeleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete(organizationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementorganizationsApi.DeleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete: " + e.Message );
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

            var apiInstance = new ManagementorganizationsApi();
            var organizationId = new Object(); // Object | 

            try
            {
                // Get An Organization
                GetOrganizationResponseModel result = apiInstance.GetAnOrganizationV3ManagementOrganizationsOrganizationIdGet(organizationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementorganizationsApi.GetAnOrganizationV3ManagementOrganizationsOrganizationIdGet: " + e.Message );
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

            var apiInstance = new ManagementorganizationsApi();

            try
            {
                // List All Organizations
                ListOrganizationsResponseModel result = apiInstance.ListAllOrganizationsV3ManagementOrganizationsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementorganizationsApi.ListAllOrganizationsV3ManagementOrganizationsGet: " + e.Message );
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

            var apiInstance = new ManagementorganizationsApi();
            var organizationId = new Object(); // Object | 

            try
            {
                // List Organization Applications
                ListOrganizationApplicationsResponseModel result = apiInstance.ListOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet(organizationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ManagementorganizationsApi.ListOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet: " + e.Message );
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

            var apiInstance = new ManagementorganizationsApi();
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
                Debug.Print("Exception when calling ManagementorganizationsApi.UpdateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch: " + e.Message );
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
