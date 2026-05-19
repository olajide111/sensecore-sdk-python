# sensecore.APIKeysApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_api_key_api_v1_api_keys_post**](APIKeysApi.md#create_api_key_api_v1_api_keys_post) | **POST** /api/v1/api-keys | Create Api Key
[**list_api_keys_api_v1_api_keys_get**](APIKeysApi.md#list_api_keys_api_v1_api_keys_get) | **GET** /api/v1/api-keys | List Api Keys
[**revoke_api_key_api_v1_api_keys_key_id_delete**](APIKeysApi.md#revoke_api_key_api_v1_api_keys_key_id_delete) | **DELETE** /api/v1/api-keys/{key_id} | Revoke Api Key
[**rotate_api_key_api_v1_api_keys_key_id_rotate_post**](APIKeysApi.md#rotate_api_key_api_v1_api_keys_key_id_rotate_post) | **POST** /api/v1/api-keys/{key_id}/rotate | Rotate Api Key
[**whoami_api_v1_api_keys_whoami_get**](APIKeysApi.md#whoami_api_v1_api_keys_whoami_get) | **GET** /api/v1/api-keys/whoami | Whoami


# **create_api_key_api_v1_api_keys_post**
> APIKeyCreatedResponse create_api_key_api_v1_api_keys_post(create_api_key_request)

Create Api Key

Create a new API key. Plaintext returned ONCE in `full_key` — store it now.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.api_key_created_response import APIKeyCreatedResponse
from sensecore.models.create_api_key_request import CreateAPIKeyRequest
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
    api_instance = sensecore.APIKeysApi(api_client)
    create_api_key_request = sensecore.CreateAPIKeyRequest() # CreateAPIKeyRequest | 

    try:
        # Create Api Key
        api_response = api_instance.create_api_key_api_v1_api_keys_post(create_api_key_request)
        print("The response of APIKeysApi->create_api_key_api_v1_api_keys_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling APIKeysApi->create_api_key_api_v1_api_keys_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **create_api_key_request** | [**CreateAPIKeyRequest**](CreateAPIKeyRequest.md)|  | 

### Return type

[**APIKeyCreatedResponse**](APIKeyCreatedResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_api_keys_api_v1_api_keys_get**
> List[APIKeyResponse] list_api_keys_api_v1_api_keys_get(include_revoked=include_revoked)

List Api Keys

List API keys for the caller's org. Never returns plaintext or hashes.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.api_key_response import APIKeyResponse
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
    api_instance = sensecore.APIKeysApi(api_client)
    include_revoked = False # bool |  (optional) (default to False)

    try:
        # List Api Keys
        api_response = api_instance.list_api_keys_api_v1_api_keys_get(include_revoked=include_revoked)
        print("The response of APIKeysApi->list_api_keys_api_v1_api_keys_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling APIKeysApi->list_api_keys_api_v1_api_keys_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **include_revoked** | **bool**|  | [optional] [default to False]

### Return type

[**List[APIKeyResponse]**](APIKeyResponse.md)

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

# **revoke_api_key_api_v1_api_keys_key_id_delete**
> revoke_api_key_api_v1_api_keys_key_id_delete(key_id)

Revoke Api Key

Revoke a key. Soft-delete — revoked_at set, row preserved for audit.

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
    api_instance = sensecore.APIKeysApi(api_client)
    key_id = 'key_id_example' # str | 

    try:
        # Revoke Api Key
        api_instance.revoke_api_key_api_v1_api_keys_key_id_delete(key_id)
    except Exception as e:
        print("Exception when calling APIKeysApi->revoke_api_key_api_v1_api_keys_key_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key_id** | **str**|  | 

### Return type

void (empty response body)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **rotate_api_key_api_v1_api_keys_key_id_rotate_post**
> APIKeyCreatedResponse rotate_api_key_api_v1_api_keys_key_id_rotate_post(key_id)

Rotate Api Key

Atomic revoke + reissue. Old key invalidated immediately, name preserved.
New plaintext returned ONCE — store it now.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.api_key_created_response import APIKeyCreatedResponse
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
    api_instance = sensecore.APIKeysApi(api_client)
    key_id = 'key_id_example' # str | 

    try:
        # Rotate Api Key
        api_response = api_instance.rotate_api_key_api_v1_api_keys_key_id_rotate_post(key_id)
        print("The response of APIKeysApi->rotate_api_key_api_v1_api_keys_key_id_rotate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling APIKeysApi->rotate_api_key_api_v1_api_keys_key_id_rotate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key_id** | **str**|  | 

### Return type

[**APIKeyCreatedResponse**](APIKeyCreatedResponse.md)

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

# **whoami_api_v1_api_keys_whoami_get**
> object whoami_api_v1_api_keys_whoami_get(x_api_key=x_api_key)

Whoami

Return how the system sees the current caller.

Accepts JWT (Authorization: Bearer) OR X-API-Key. Useful for confirming
a key works without making a real data-plane call, and for debugging
auth flows. Unlike the other routes in this module, this endpoint
deliberately uses the hybrid dep — so an API-key holder can verify
their own key by hitting /whoami before relying on it elsewhere.

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
    api_instance = sensecore.APIKeysApi(api_client)
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Whoami
        api_response = api_instance.whoami_api_v1_api_keys_whoami_get(x_api_key=x_api_key)
        print("The response of APIKeysApi->whoami_api_v1_api_keys_whoami_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling APIKeysApi->whoami_api_v1_api_keys_whoami_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_api_key** | **str**|  | [optional] 

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

