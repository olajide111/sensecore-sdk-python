# sensecore.EmailProvidersApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**activate_provider_api_v1_admin_email_providers_kind_activate_post**](EmailProvidersApi.md#activate_provider_api_v1_admin_email_providers_kind_activate_post) | **POST** /api/v1/admin/email-providers/{kind}/activate | Activate Provider
[**activate_provider_api_v1_admin_email_providers_kind_activate_post_0**](EmailProvidersApi.md#activate_provider_api_v1_admin_email_providers_kind_activate_post_0) | **POST** /api/v1/admin/email-providers/{kind}/activate | Activate Provider
[**get_provider_api_v1_admin_email_providers_kind_get**](EmailProvidersApi.md#get_provider_api_v1_admin_email_providers_kind_get) | **GET** /api/v1/admin/email-providers/{kind} | Get Provider
[**get_provider_api_v1_admin_email_providers_kind_get_0**](EmailProvidersApi.md#get_provider_api_v1_admin_email_providers_kind_get_0) | **GET** /api/v1/admin/email-providers/{kind} | Get Provider
[**get_registry_api_v1_admin_email_providers_types_registry_get**](EmailProvidersApi.md#get_registry_api_v1_admin_email_providers_types_registry_get) | **GET** /api/v1/admin/email-providers/types/registry | Get Registry
[**get_registry_api_v1_admin_email_providers_types_registry_get_0**](EmailProvidersApi.md#get_registry_api_v1_admin_email_providers_types_registry_get_0) | **GET** /api/v1/admin/email-providers/types/registry | Get Registry
[**list_providers_api_v1_admin_email_providers_get**](EmailProvidersApi.md#list_providers_api_v1_admin_email_providers_get) | **GET** /api/v1/admin/email-providers | List Providers
[**list_providers_api_v1_admin_email_providers_get_0**](EmailProvidersApi.md#list_providers_api_v1_admin_email_providers_get_0) | **GET** /api/v1/admin/email-providers | List Providers
[**test_provider_api_v1_admin_email_providers_kind_test_post**](EmailProvidersApi.md#test_provider_api_v1_admin_email_providers_kind_test_post) | **POST** /api/v1/admin/email-providers/{kind}/test | Test Provider
[**test_provider_api_v1_admin_email_providers_kind_test_post_0**](EmailProvidersApi.md#test_provider_api_v1_admin_email_providers_kind_test_post_0) | **POST** /api/v1/admin/email-providers/{kind}/test | Test Provider
[**update_provider_api_v1_admin_email_providers_kind_put**](EmailProvidersApi.md#update_provider_api_v1_admin_email_providers_kind_put) | **PUT** /api/v1/admin/email-providers/{kind} | Update Provider
[**update_provider_api_v1_admin_email_providers_kind_put_0**](EmailProvidersApi.md#update_provider_api_v1_admin_email_providers_kind_put_0) | **PUT** /api/v1/admin/email-providers/{kind} | Update Provider


# **activate_provider_api_v1_admin_email_providers_kind_activate_post**
> object activate_provider_api_v1_admin_email_providers_kind_activate_post(kind)

Activate Provider

Make this provider the active one. Deactivates all others atomically.

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
    api_instance = sensecore.EmailProvidersApi(api_client)
    kind = 'kind_example' # str | 

    try:
        # Activate Provider
        api_response = api_instance.activate_provider_api_v1_admin_email_providers_kind_activate_post(kind)
        print("The response of EmailProvidersApi->activate_provider_api_v1_admin_email_providers_kind_activate_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->activate_provider_api_v1_admin_email_providers_kind_activate_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **kind** | **str**|  | 

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

# **activate_provider_api_v1_admin_email_providers_kind_activate_post_0**
> object activate_provider_api_v1_admin_email_providers_kind_activate_post_0(kind)

Activate Provider

Make this provider the active one. Deactivates all others atomically.

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
    api_instance = sensecore.EmailProvidersApi(api_client)
    kind = 'kind_example' # str | 

    try:
        # Activate Provider
        api_response = api_instance.activate_provider_api_v1_admin_email_providers_kind_activate_post_0(kind)
        print("The response of EmailProvidersApi->activate_provider_api_v1_admin_email_providers_kind_activate_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->activate_provider_api_v1_admin_email_providers_kind_activate_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **kind** | **str**|  | 

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

# **get_provider_api_v1_admin_email_providers_kind_get**
> object get_provider_api_v1_admin_email_providers_kind_get(kind, redacted=redacted)

Get Provider

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
    api_instance = sensecore.EmailProvidersApi(api_client)
    kind = 'kind_example' # str | 
    redacted = False # bool |  (optional) (default to False)

    try:
        # Get Provider
        api_response = api_instance.get_provider_api_v1_admin_email_providers_kind_get(kind, redacted=redacted)
        print("The response of EmailProvidersApi->get_provider_api_v1_admin_email_providers_kind_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->get_provider_api_v1_admin_email_providers_kind_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **kind** | **str**|  | 
 **redacted** | **bool**|  | [optional] [default to False]

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

# **get_provider_api_v1_admin_email_providers_kind_get_0**
> object get_provider_api_v1_admin_email_providers_kind_get_0(kind, redacted=redacted)

Get Provider

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
    api_instance = sensecore.EmailProvidersApi(api_client)
    kind = 'kind_example' # str | 
    redacted = False # bool |  (optional) (default to False)

    try:
        # Get Provider
        api_response = api_instance.get_provider_api_v1_admin_email_providers_kind_get_0(kind, redacted=redacted)
        print("The response of EmailProvidersApi->get_provider_api_v1_admin_email_providers_kind_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->get_provider_api_v1_admin_email_providers_kind_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **kind** | **str**|  | 
 **redacted** | **bool**|  | [optional] [default to False]

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

# **get_registry_api_v1_admin_email_providers_types_registry_get**
> object get_registry_api_v1_admin_email_providers_types_registry_get()

Get Registry

Returns the provider type schemas. Used by the admin UI to render the
correct config form for each provider type.

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
    api_instance = sensecore.EmailProvidersApi(api_client)

    try:
        # Get Registry
        api_response = api_instance.get_registry_api_v1_admin_email_providers_types_registry_get()
        print("The response of EmailProvidersApi->get_registry_api_v1_admin_email_providers_types_registry_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->get_registry_api_v1_admin_email_providers_types_registry_get: %s\n" % e)
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

# **get_registry_api_v1_admin_email_providers_types_registry_get_0**
> object get_registry_api_v1_admin_email_providers_types_registry_get_0()

Get Registry

Returns the provider type schemas. Used by the admin UI to render the
correct config form for each provider type.

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
    api_instance = sensecore.EmailProvidersApi(api_client)

    try:
        # Get Registry
        api_response = api_instance.get_registry_api_v1_admin_email_providers_types_registry_get_0()
        print("The response of EmailProvidersApi->get_registry_api_v1_admin_email_providers_types_registry_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->get_registry_api_v1_admin_email_providers_types_registry_get_0: %s\n" % e)
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

# **list_providers_api_v1_admin_email_providers_get**
> object list_providers_api_v1_admin_email_providers_get()

List Providers

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
    api_instance = sensecore.EmailProvidersApi(api_client)

    try:
        # List Providers
        api_response = api_instance.list_providers_api_v1_admin_email_providers_get()
        print("The response of EmailProvidersApi->list_providers_api_v1_admin_email_providers_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->list_providers_api_v1_admin_email_providers_get: %s\n" % e)
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

# **list_providers_api_v1_admin_email_providers_get_0**
> object list_providers_api_v1_admin_email_providers_get_0()

List Providers

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
    api_instance = sensecore.EmailProvidersApi(api_client)

    try:
        # List Providers
        api_response = api_instance.list_providers_api_v1_admin_email_providers_get_0()
        print("The response of EmailProvidersApi->list_providers_api_v1_admin_email_providers_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->list_providers_api_v1_admin_email_providers_get_0: %s\n" % e)
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

# **test_provider_api_v1_admin_email_providers_kind_test_post**
> object test_provider_api_v1_admin_email_providers_kind_test_post(kind, body=body)

Test Provider

Test the provider's authentication / reachability without sending an
actual email. Body is optional — pass `{"config": {...}}` to test
UNSAVED config; otherwise tests the saved config.

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
    api_instance = sensecore.EmailProvidersApi(api_client)
    kind = 'kind_example' # str | 
    body = None # object |  (optional)

    try:
        # Test Provider
        api_response = api_instance.test_provider_api_v1_admin_email_providers_kind_test_post(kind, body=body)
        print("The response of EmailProvidersApi->test_provider_api_v1_admin_email_providers_kind_test_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->test_provider_api_v1_admin_email_providers_kind_test_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **kind** | **str**|  | 
 **body** | **object**|  | [optional] 

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

# **test_provider_api_v1_admin_email_providers_kind_test_post_0**
> object test_provider_api_v1_admin_email_providers_kind_test_post_0(kind, body=body)

Test Provider

Test the provider's authentication / reachability without sending an
actual email. Body is optional — pass `{"config": {...}}` to test
UNSAVED config; otherwise tests the saved config.

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
    api_instance = sensecore.EmailProvidersApi(api_client)
    kind = 'kind_example' # str | 
    body = None # object |  (optional)

    try:
        # Test Provider
        api_response = api_instance.test_provider_api_v1_admin_email_providers_kind_test_post_0(kind, body=body)
        print("The response of EmailProvidersApi->test_provider_api_v1_admin_email_providers_kind_test_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->test_provider_api_v1_admin_email_providers_kind_test_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **kind** | **str**|  | 
 **body** | **object**|  | [optional] 

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

# **update_provider_api_v1_admin_email_providers_kind_put**
> object update_provider_api_v1_admin_email_providers_kind_put(kind, body)

Update Provider

Body:
  {
    "config": { ... provider-specific ... },
    "notes":  "free text",          # optional
    "name":   "Custom name"          # optional, defaults preserved
  }

Sensitive fields that come in masked (••••XXXX) keep their existing value.

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
    api_instance = sensecore.EmailProvidersApi(api_client)
    kind = 'kind_example' # str | 
    body = None # object | 

    try:
        # Update Provider
        api_response = api_instance.update_provider_api_v1_admin_email_providers_kind_put(kind, body)
        print("The response of EmailProvidersApi->update_provider_api_v1_admin_email_providers_kind_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->update_provider_api_v1_admin_email_providers_kind_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **kind** | **str**|  | 
 **body** | **object**|  | 

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

# **update_provider_api_v1_admin_email_providers_kind_put_0**
> object update_provider_api_v1_admin_email_providers_kind_put_0(kind, body)

Update Provider

Body:
  {
    "config": { ... provider-specific ... },
    "notes":  "free text",          # optional
    "name":   "Custom name"          # optional, defaults preserved
  }

Sensitive fields that come in masked (••••XXXX) keep their existing value.

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
    api_instance = sensecore.EmailProvidersApi(api_client)
    kind = 'kind_example' # str | 
    body = None # object | 

    try:
        # Update Provider
        api_response = api_instance.update_provider_api_v1_admin_email_providers_kind_put_0(kind, body)
        print("The response of EmailProvidersApi->update_provider_api_v1_admin_email_providers_kind_put_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailProvidersApi->update_provider_api_v1_admin_email_providers_kind_put_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **kind** | **str**|  | 
 **body** | **object**|  | 

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

