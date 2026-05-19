# sensecore.NotificationsApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**clear_notifications_api_v1_notifications_delete**](NotificationsApi.md#clear_notifications_api_v1_notifications_delete) | **DELETE** /api/v1/notifications | Clear Notifications
[**clear_notifications_api_v1_notifications_delete_0**](NotificationsApi.md#clear_notifications_api_v1_notifications_delete_0) | **DELETE** /api/v1/notifications | Clear Notifications
[**list_notifications_api_v1_notifications_get**](NotificationsApi.md#list_notifications_api_v1_notifications_get) | **GET** /api/v1/notifications | List Notifications
[**list_notifications_api_v1_notifications_get_0**](NotificationsApi.md#list_notifications_api_v1_notifications_get_0) | **GET** /api/v1/notifications | List Notifications
[**mark_read_api_v1_notifications_read_post**](NotificationsApi.md#mark_read_api_v1_notifications_read_post) | **POST** /api/v1/notifications/read | Mark Read
[**mark_read_api_v1_notifications_read_post_0**](NotificationsApi.md#mark_read_api_v1_notifications_read_post_0) | **POST** /api/v1/notifications/read | Mark Read
[**unread_count_api_v1_notifications_unread_count_get**](NotificationsApi.md#unread_count_api_v1_notifications_unread_count_get) | **GET** /api/v1/notifications/unread-count | Unread Count
[**unread_count_api_v1_notifications_unread_count_get_0**](NotificationsApi.md#unread_count_api_v1_notifications_unread_count_get_0) | **GET** /api/v1/notifications/unread-count | Unread Count


# **clear_notifications_api_v1_notifications_delete**
> object clear_notifications_api_v1_notifications_delete()

Clear Notifications

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
    api_instance = sensecore.NotificationsApi(api_client)

    try:
        # Clear Notifications
        api_response = api_instance.clear_notifications_api_v1_notifications_delete()
        print("The response of NotificationsApi->clear_notifications_api_v1_notifications_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->clear_notifications_api_v1_notifications_delete: %s\n" % e)
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

# **clear_notifications_api_v1_notifications_delete_0**
> object clear_notifications_api_v1_notifications_delete_0()

Clear Notifications

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
    api_instance = sensecore.NotificationsApi(api_client)

    try:
        # Clear Notifications
        api_response = api_instance.clear_notifications_api_v1_notifications_delete_0()
        print("The response of NotificationsApi->clear_notifications_api_v1_notifications_delete_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->clear_notifications_api_v1_notifications_delete_0: %s\n" % e)
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

# **list_notifications_api_v1_notifications_get**
> object list_notifications_api_v1_notifications_get(limit=limit)

List Notifications

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
    api_instance = sensecore.NotificationsApi(api_client)
    limit = 50 # int |  (optional) (default to 50)

    try:
        # List Notifications
        api_response = api_instance.list_notifications_api_v1_notifications_get(limit=limit)
        print("The response of NotificationsApi->list_notifications_api_v1_notifications_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->list_notifications_api_v1_notifications_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]

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

# **list_notifications_api_v1_notifications_get_0**
> object list_notifications_api_v1_notifications_get_0(limit=limit)

List Notifications

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
    api_instance = sensecore.NotificationsApi(api_client)
    limit = 50 # int |  (optional) (default to 50)

    try:
        # List Notifications
        api_response = api_instance.list_notifications_api_v1_notifications_get_0(limit=limit)
        print("The response of NotificationsApi->list_notifications_api_v1_notifications_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->list_notifications_api_v1_notifications_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **limit** | **int**|  | [optional] [default to 50]

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

# **mark_read_api_v1_notifications_read_post**
> object mark_read_api_v1_notifications_read_post(body)

Mark Read

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
    api_instance = sensecore.NotificationsApi(api_client)
    body = None # object | 

    try:
        # Mark Read
        api_response = api_instance.mark_read_api_v1_notifications_read_post(body)
        print("The response of NotificationsApi->mark_read_api_v1_notifications_read_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->mark_read_api_v1_notifications_read_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **mark_read_api_v1_notifications_read_post_0**
> object mark_read_api_v1_notifications_read_post_0(body)

Mark Read

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
    api_instance = sensecore.NotificationsApi(api_client)
    body = None # object | 

    try:
        # Mark Read
        api_response = api_instance.mark_read_api_v1_notifications_read_post_0(body)
        print("The response of NotificationsApi->mark_read_api_v1_notifications_read_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->mark_read_api_v1_notifications_read_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | 

### Return type

**object**

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **unread_count_api_v1_notifications_unread_count_get**
> object unread_count_api_v1_notifications_unread_count_get()

Unread Count

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
    api_instance = sensecore.NotificationsApi(api_client)

    try:
        # Unread Count
        api_response = api_instance.unread_count_api_v1_notifications_unread_count_get()
        print("The response of NotificationsApi->unread_count_api_v1_notifications_unread_count_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->unread_count_api_v1_notifications_unread_count_get: %s\n" % e)
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

# **unread_count_api_v1_notifications_unread_count_get_0**
> object unread_count_api_v1_notifications_unread_count_get_0()

Unread Count

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
    api_instance = sensecore.NotificationsApi(api_client)

    try:
        # Unread Count
        api_response = api_instance.unread_count_api_v1_notifications_unread_count_get_0()
        print("The response of NotificationsApi->unread_count_api_v1_notifications_unread_count_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling NotificationsApi->unread_count_api_v1_notifications_unread_count_get_0: %s\n" % e)
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

