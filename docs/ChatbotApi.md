# IO.Swagger.Api.ChatbotApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreateAConversationV3ChatbotConversationsPost**](ChatbotApi.md#createaconversationv3chatbotconversationspost) | **POST** /v3/chatbot/conversations | Create A Conversation
[**CreateANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost**](ChatbotApi.md#createanewmessageinaconversationv3chatbotconversationsconversationidmessagespost) | **POST** /v3/chatbot/conversations/{conversation_id}/messages | Create A New Message In A Conversation
[**DeleteAConversationV3ChatbotConversationsConversationIdDelete**](ChatbotApi.md#deleteaconversationv3chatbotconversationsconversationiddelete) | **DELETE** /v3/chatbot/conversations/{conversation_id} | Delete A Conversation
[**GetAConversationV3ChatbotConversationsConversationIdGet**](ChatbotApi.md#getaconversationv3chatbotconversationsconversationidget) | **GET** /v3/chatbot/conversations/{conversation_id} | Get A Conversation
[**ListAllConversationsV3ChatbotConversationsGet**](ChatbotApi.md#listallconversationsv3chatbotconversationsget) | **GET** /v3/chatbot/conversations | List All Conversations
[**ListConversationMessagesV3ChatbotConversationsConversationIdMessagesGet**](ChatbotApi.md#listconversationmessagesv3chatbotconversationsconversationidmessagesget) | **GET** /v3/chatbot/conversations/{conversation_id}/messages | List Conversation Messages
[**UpdateAConversationV3ChatbotConversationsConversationIdPatch**](ChatbotApi.md#updateaconversationv3chatbotconversationsconversationidpatch) | **PATCH** /v3/chatbot/conversations/{conversation_id} | Update A Conversation

<a name="createaconversationv3chatbotconversationspost"></a>
# **CreateAConversationV3ChatbotConversationsPost**
> CreateConversationResponseModel CreateAConversationV3ChatbotConversationsPost (CreateConversationRequestModel body)

Create A Conversation

Creates a conversation.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateAConversationV3ChatbotConversationsPostExample
    {
        public void main()
        {

            var apiInstance = new ChatbotApi();
            var body = new CreateConversationRequestModel(); // CreateConversationRequestModel | 

            try
            {
                // Create A Conversation
                CreateConversationResponseModel result = apiInstance.CreateAConversationV3ChatbotConversationsPost(body);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ChatbotApi.CreateAConversationV3ChatbotConversationsPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateConversationRequestModel**](CreateConversationRequestModel.md)|  | 

### Return type

[**CreateConversationResponseModel**](CreateConversationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="createanewmessageinaconversationv3chatbotconversationsconversationidmessagespost"></a>
# **CreateANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost**
> CreateConversationMessageResponseModel CreateANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost (CreateConversationMessageRequestModel body, Object conversationId)

Create A New Message In A Conversation

Creates a new message in a conversation along with a completion from the LLM.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class CreateANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPostExample
    {
        public void main()
        {

            var apiInstance = new ChatbotApi();
            var body = new CreateConversationMessageRequestModel(); // CreateConversationMessageRequestModel | 
            var conversationId = new Object(); // Object | 

            try
            {
                // Create A New Message In A Conversation
                CreateConversationMessageResponseModel result = apiInstance.CreateANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost(body, conversationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ChatbotApi.CreateANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateConversationMessageRequestModel**](CreateConversationMessageRequestModel.md)|  | 
 **conversationId** | [**Object**](Object.md)|  | 

### Return type

[**CreateConversationMessageResponseModel**](CreateConversationMessageResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="deleteaconversationv3chatbotconversationsconversationiddelete"></a>
# **DeleteAConversationV3ChatbotConversationsConversationIdDelete**
> Object DeleteAConversationV3ChatbotConversationsConversationIdDelete (Object conversationId)

Delete A Conversation

Deletes the conversation specified in `conversation_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class DeleteAConversationV3ChatbotConversationsConversationIdDeleteExample
    {
        public void main()
        {

            var apiInstance = new ChatbotApi();
            var conversationId = new Object(); // Object | 

            try
            {
                // Delete A Conversation
                Object result = apiInstance.DeleteAConversationV3ChatbotConversationsConversationIdDelete(conversationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ChatbotApi.DeleteAConversationV3ChatbotConversationsConversationIdDelete: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversationId** | [**Object**](Object.md)|  | 

### Return type

**Object**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="getaconversationv3chatbotconversationsconversationidget"></a>
# **GetAConversationV3ChatbotConversationsConversationIdGet**
> GetConversationResponseModel GetAConversationV3ChatbotConversationsConversationIdGet (Object conversationId)

Get A Conversation

Returns a conversation matching the provided `conversation_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class GetAConversationV3ChatbotConversationsConversationIdGetExample
    {
        public void main()
        {

            var apiInstance = new ChatbotApi();
            var conversationId = new Object(); // Object | 

            try
            {
                // Get A Conversation
                GetConversationResponseModel result = apiInstance.GetAConversationV3ChatbotConversationsConversationIdGet(conversationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ChatbotApi.GetAConversationV3ChatbotConversationsConversationIdGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversationId** | [**Object**](Object.md)|  | 

### Return type

[**GetConversationResponseModel**](GetConversationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="listallconversationsv3chatbotconversationsget"></a>
# **ListAllConversationsV3ChatbotConversationsGet**
> ListConversationsResponseModel ListAllConversationsV3ChatbotConversationsGet ()

List All Conversations

Lists all conversations.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ListAllConversationsV3ChatbotConversationsGetExample
    {
        public void main()
        {

            var apiInstance = new ChatbotApi();

            try
            {
                // List All Conversations
                ListConversationsResponseModel result = apiInstance.ListAllConversationsV3ChatbotConversationsGet();
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ChatbotApi.ListAllConversationsV3ChatbotConversationsGet: " + e.Message );
            }
        }
    }
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListConversationsResponseModel**](ListConversationsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="listconversationmessagesv3chatbotconversationsconversationidmessagesget"></a>
# **ListConversationMessagesV3ChatbotConversationsConversationIdMessagesGet**
> ListConversationMessagesResponseModel ListConversationMessagesV3ChatbotConversationsConversationIdMessagesGet (Object conversationId)

List Conversation Messages

Lists all messages associated with a conversation specified in `conversation_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class ListConversationMessagesV3ChatbotConversationsConversationIdMessagesGetExample
    {
        public void main()
        {

            var apiInstance = new ChatbotApi();
            var conversationId = new Object(); // Object | 

            try
            {
                // List Conversation Messages
                ListConversationMessagesResponseModel result = apiInstance.ListConversationMessagesV3ChatbotConversationsConversationIdMessagesGet(conversationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ChatbotApi.ListConversationMessagesV3ChatbotConversationsConversationIdMessagesGet: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversationId** | [**Object**](Object.md)|  | 

### Return type

[**ListConversationMessagesResponseModel**](ListConversationMessagesResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
<a name="updateaconversationv3chatbotconversationsconversationidpatch"></a>
# **UpdateAConversationV3ChatbotConversationsConversationIdPatch**
> UpdateConversationResponseModel UpdateAConversationV3ChatbotConversationsConversationIdPatch (UpdateConversationRequestModel body, Object conversationId)

Update A Conversation

Updates the conversation specified in `conversation_id`.

### Example
```csharp
using System;
using System.Diagnostics;
using IO.Swagger.Api;
using IO.Swagger.Client;
using IO.Swagger.Model;

namespace Example
{
    public class UpdateAConversationV3ChatbotConversationsConversationIdPatchExample
    {
        public void main()
        {

            var apiInstance = new ChatbotApi();
            var body = new UpdateConversationRequestModel(); // UpdateConversationRequestModel | 
            var conversationId = new Object(); // Object | 

            try
            {
                // Update A Conversation
                UpdateConversationResponseModel result = apiInstance.UpdateAConversationV3ChatbotConversationsConversationIdPatch(body, conversationId);
                Debug.WriteLine(result);
            }
            catch (Exception e)
            {
                Debug.Print("Exception when calling ChatbotApi.UpdateAConversationV3ChatbotConversationsConversationIdPatch: " + e.Message );
            }
        }
    }
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UpdateConversationRequestModel**](UpdateConversationRequestModel.md)|  | 
 **conversationId** | [**Object**](Object.md)|  | 

### Return type

[**UpdateConversationResponseModel**](UpdateConversationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)
