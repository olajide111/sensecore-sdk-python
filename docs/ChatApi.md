# sensecore.ChatApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**admin_chat_stats_api_v1_chat_admin_stats_get**](ChatApi.md#admin_chat_stats_api_v1_chat_admin_stats_get) | **GET** /api/v1/chat/admin/stats | Admin Chat Stats
[**admin_conversation_detail_api_v1_chat_admin_conversations_conversation_id_get**](ChatApi.md#admin_conversation_detail_api_v1_chat_admin_conversations_conversation_id_get) | **GET** /api/v1/chat/admin/conversations/{conversation_id} | Admin Conversation Detail
[**admin_get_chat_config_api_v1_chat_admin_config_get**](ChatApi.md#admin_get_chat_config_api_v1_chat_admin_config_get) | **GET** /api/v1/chat/admin/config | Admin Get Chat Config
[**admin_get_widgets_api_v1_chat_admin_widgets_get**](ChatApi.md#admin_get_widgets_api_v1_chat_admin_widgets_get) | **GET** /api/v1/chat/admin/widgets | Admin Get Widgets
[**admin_list_conversations_api_v1_chat_admin_conversations_get**](ChatApi.md#admin_list_conversations_api_v1_chat_admin_conversations_get) | **GET** /api/v1/chat/admin/conversations | Admin List Conversations
[**admin_list_leads_api_v1_chat_admin_leads_get**](ChatApi.md#admin_list_leads_api_v1_chat_admin_leads_get) | **GET** /api/v1/chat/admin/leads | Admin List Leads
[**admin_update_chat_config_api_v1_chat_admin_config_put**](ChatApi.md#admin_update_chat_config_api_v1_chat_admin_config_put) | **PUT** /api/v1/chat/admin/config | Admin Update Chat Config
[**admin_update_lead_status_api_v1_chat_admin_leads_lead_id_status_put**](ChatApi.md#admin_update_lead_status_api_v1_chat_admin_leads_lead_id_status_put) | **PUT** /api/v1/chat/admin/leads/{lead_id}/status | Admin Update Lead Status
[**admin_update_widget_prompt_api_v1_chat_admin_widgets_widget_id_prompt_put**](ChatApi.md#admin_update_widget_prompt_api_v1_chat_admin_widgets_widget_id_prompt_put) | **PUT** /api/v1/chat/admin/widgets/{widget_id}/prompt | Admin Update Widget Prompt
[**capture_chat_lead_api_v1_chat_lead_post**](ChatApi.md#capture_chat_lead_api_v1_chat_lead_post) | **POST** /api/v1/chat/lead | Capture Chat Lead
[**chat_message_api_v1_chat_message_post**](ChatApi.md#chat_message_api_v1_chat_message_post) | **POST** /api/v1/chat/message | Chat Message
[**chat_message_authenticated_api_v1_chat_message_authenticated_post**](ChatApi.md#chat_message_authenticated_api_v1_chat_message_authenticated_post) | **POST** /api/v1/chat/message/authenticated | Chat Message Authenticated
[**get_chat_config_api_v1_chat_config_get**](ChatApi.md#get_chat_config_api_v1_chat_config_get) | **GET** /api/v1/chat/config | Get Chat Config
[**get_chat_history_api_v1_chat_history_session_id_get**](ChatApi.md#get_chat_history_api_v1_chat_history_session_id_get) | **GET** /api/v1/chat/history/{session_id} | Get Chat History


# **admin_chat_stats_api_v1_chat_admin_stats_get**
> object admin_chat_stats_api_v1_chat_admin_stats_get()

Admin Chat Stats

Admin: chat dashboard stats.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)

    try:
        # Admin Chat Stats
        api_response = api_instance.admin_chat_stats_api_v1_chat_admin_stats_get()
        print("The response of ChatApi->admin_chat_stats_api_v1_chat_admin_stats_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->admin_chat_stats_api_v1_chat_admin_stats_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_conversation_detail_api_v1_chat_admin_conversations_conversation_id_get**
> object admin_conversation_detail_api_v1_chat_admin_conversations_conversation_id_get(conversation_id)

Admin Conversation Detail

Admin: view a specific conversation with messages.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)
    conversation_id = 'conversation_id_example' # str | 

    try:
        # Admin Conversation Detail
        api_response = api_instance.admin_conversation_detail_api_v1_chat_admin_conversations_conversation_id_get(conversation_id)
        print("The response of ChatApi->admin_conversation_detail_api_v1_chat_admin_conversations_conversation_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->admin_conversation_detail_api_v1_chat_admin_conversations_conversation_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversation_id** | **str**|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_get_chat_config_api_v1_chat_admin_config_get**
> object admin_get_chat_config_api_v1_chat_admin_config_get()

Admin Get Chat Config

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)

    try:
        # Admin Get Chat Config
        api_response = api_instance.admin_get_chat_config_api_v1_chat_admin_config_get()
        print("The response of ChatApi->admin_get_chat_config_api_v1_chat_admin_config_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->admin_get_chat_config_api_v1_chat_admin_config_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_get_widgets_api_v1_chat_admin_widgets_get**
> object admin_get_widgets_api_v1_chat_admin_widgets_get()

Admin Get Widgets

Admin: list all chat widgets with their system prompts.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)

    try:
        # Admin Get Widgets
        api_response = api_instance.admin_get_widgets_api_v1_chat_admin_widgets_get()
        print("The response of ChatApi->admin_get_widgets_api_v1_chat_admin_widgets_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->admin_get_widgets_api_v1_chat_admin_widgets_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_list_conversations_api_v1_chat_admin_conversations_get**
> object admin_list_conversations_api_v1_chat_admin_conversations_get(limit=limit, offset=offset, source=source, has_lead=has_lead)

Admin List Conversations

Admin: list all conversations.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    offset = 0 # int |  (optional) (default to 0)
    source = 'source_example' # str |  (optional)
    has_lead = True # bool |  (optional)

    try:
        # Admin List Conversations
        api_response = api_instance.admin_list_conversations_api_v1_chat_admin_conversations_get(limit=limit, offset=offset, source=source, has_lead=has_lead)
        print("The response of ChatApi->admin_list_conversations_api_v1_chat_admin_conversations_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->admin_list_conversations_api_v1_chat_admin_conversations_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **offset** | **int**|  | [optional] [default to 0]
 **source** | **str**|  | [optional] 
 **has_lead** | **bool**|  | [optional] 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_list_leads_api_v1_chat_admin_leads_get**
> object admin_list_leads_api_v1_chat_admin_leads_get(limit=limit, offset=offset, status=status)

Admin List Leads

Admin: list all captured leads.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)
    limit = 50 # int |  (optional) (default to 50)
    offset = 0 # int |  (optional) (default to 0)
    status = 'status_example' # str |  (optional)

    try:
        # Admin List Leads
        api_response = api_instance.admin_list_leads_api_v1_chat_admin_leads_get(limit=limit, offset=offset, status=status)
        print("The response of ChatApi->admin_list_leads_api_v1_chat_admin_leads_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->admin_list_leads_api_v1_chat_admin_leads_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]
 **offset** | **int**|  | [optional] [default to 0]
 **status** | **str**|  | [optional] 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_update_chat_config_api_v1_chat_admin_config_put**
> object admin_update_chat_config_api_v1_chat_admin_config_put()

Admin Update Chat Config

Admin: update chat settings.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)

    try:
        # Admin Update Chat Config
        api_response = api_instance.admin_update_chat_config_api_v1_chat_admin_config_put()
        print("The response of ChatApi->admin_update_chat_config_api_v1_chat_admin_config_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->admin_update_chat_config_api_v1_chat_admin_config_put: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_update_lead_status_api_v1_chat_admin_leads_lead_id_status_put**
> object admin_update_lead_status_api_v1_chat_admin_leads_lead_id_status_put(lead_id)

Admin Update Lead Status

Admin: update lead status.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)
    lead_id = 'lead_id_example' # str | 

    try:
        # Admin Update Lead Status
        api_response = api_instance.admin_update_lead_status_api_v1_chat_admin_leads_lead_id_status_put(lead_id)
        print("The response of ChatApi->admin_update_lead_status_api_v1_chat_admin_leads_lead_id_status_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->admin_update_lead_status_api_v1_chat_admin_leads_lead_id_status_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lead_id** | **str**|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_update_widget_prompt_api_v1_chat_admin_widgets_widget_id_prompt_put**
> object admin_update_widget_prompt_api_v1_chat_admin_widgets_widget_id_prompt_put(widget_id)

Admin Update Widget Prompt

Admin: update a widget's system_prompt. Takes effect on next message.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

configuration.access_token = os.environ["ACCESS_TOKEN"]

# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)
    widget_id = 'widget_id_example' # str | 

    try:
        # Admin Update Widget Prompt
        api_response = api_instance.admin_update_widget_prompt_api_v1_chat_admin_widgets_widget_id_prompt_put(widget_id)
        print("The response of ChatApi->admin_update_widget_prompt_api_v1_chat_admin_widgets_widget_id_prompt_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->admin_update_widget_prompt_api_v1_chat_admin_widgets_widget_id_prompt_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **widget_id** | **str**|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **capture_chat_lead_api_v1_chat_lead_post**
> object capture_chat_lead_api_v1_chat_lead_post(lead_capture_request)

Capture Chat Lead

Capture a lead from the chat widget.

### Example


```python
import sensecore
from sensecore.models.lead_capture_request import LeadCaptureRequest
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)


# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)
    lead_capture_request = sensecore.LeadCaptureRequest() # LeadCaptureRequest | 

    try:
        # Capture Chat Lead
        api_response = api_instance.capture_chat_lead_api_v1_chat_lead_post(lead_capture_request)
        print("The response of ChatApi->capture_chat_lead_api_v1_chat_lead_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->capture_chat_lead_api_v1_chat_lead_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lead_capture_request** | [**LeadCaptureRequest**](LeadCaptureRequest.md)|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **chat_message_api_v1_chat_message_post**
> object chat_message_api_v1_chat_message_post(chat_message_request)

Chat Message

Send a message and get AI response. No auth required for marketing widget.

### Example


```python
import sensecore
from sensecore.models.chat_message_request import ChatMessageRequest
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)


# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)
    chat_message_request = sensecore.ChatMessageRequest() # ChatMessageRequest | 

    try:
        # Chat Message
        api_response = api_instance.chat_message_api_v1_chat_message_post(chat_message_request)
        print("The response of ChatApi->chat_message_api_v1_chat_message_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->chat_message_api_v1_chat_message_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **chat_message_request** | [**ChatMessageRequest**](ChatMessageRequest.md)|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **chat_message_authenticated_api_v1_chat_message_authenticated_post**
> object chat_message_authenticated_api_v1_chat_message_authenticated_post(chat_message_request)

Chat Message Authenticated

Send a message from an authenticated dashboard user.

### Example


```python
import sensecore
from sensecore.models.chat_message_request import ChatMessageRequest
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)


# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)
    chat_message_request = sensecore.ChatMessageRequest() # ChatMessageRequest | 

    try:
        # Chat Message Authenticated
        api_response = api_instance.chat_message_authenticated_api_v1_chat_message_authenticated_post(chat_message_request)
        print("The response of ChatApi->chat_message_authenticated_api_v1_chat_message_authenticated_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->chat_message_authenticated_api_v1_chat_message_authenticated_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **chat_message_request** | [**ChatMessageRequest**](ChatMessageRequest.md)|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_chat_config_api_v1_chat_config_get**
> object get_chat_config_api_v1_chat_config_get()

Get Chat Config

Public endpoint: get chat widget configuration.

### Example


```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)


# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)

    try:
        # Get Chat Config
        api_response = api_instance.get_chat_config_api_v1_chat_config_get()
        print("The response of ChatApi->get_chat_config_api_v1_chat_config_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->get_chat_config_api_v1_chat_config_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_chat_history_api_v1_chat_history_session_id_get**
> object get_chat_history_api_v1_chat_history_session_id_get(session_id)

Get Chat History

Get conversation history by session ID (for widget reload).

### Example


```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)


# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.ChatApi(api_client)
    session_id = 'session_id_example' # str | 

    try:
        # Get Chat History
        api_response = api_instance.get_chat_history_api_v1_chat_history_session_id_get(session_id)
        print("The response of ChatApi->get_chat_history_api_v1_chat_history_session_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ChatApi->get_chat_history_api_v1_chat_history_session_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **session_id** | **str**|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

