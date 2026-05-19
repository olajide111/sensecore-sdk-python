# sensecore.EmailTemplatesApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_template_api_v1_admin_email_templates_key_get**](EmailTemplatesApi.md#get_template_api_v1_admin_email_templates_key_get) | **GET** /api/v1/admin/email-templates/{key} | Get Template
[**get_template_api_v1_admin_email_templates_key_get_0**](EmailTemplatesApi.md#get_template_api_v1_admin_email_templates_key_get_0) | **GET** /api/v1/admin/email-templates/{key} | Get Template
[**list_templates_api_v1_admin_email_templates_get**](EmailTemplatesApi.md#list_templates_api_v1_admin_email_templates_get) | **GET** /api/v1/admin/email-templates | List Templates
[**list_templates_api_v1_admin_email_templates_get_0**](EmailTemplatesApi.md#list_templates_api_v1_admin_email_templates_get_0) | **GET** /api/v1/admin/email-templates | List Templates
[**preview_template_api_v1_admin_email_templates_key_preview_post**](EmailTemplatesApi.md#preview_template_api_v1_admin_email_templates_key_preview_post) | **POST** /api/v1/admin/email-templates/{key}/preview | Preview Template
[**preview_template_api_v1_admin_email_templates_key_preview_post_0**](EmailTemplatesApi.md#preview_template_api_v1_admin_email_templates_key_preview_post_0) | **POST** /api/v1/admin/email-templates/{key}/preview | Preview Template
[**reset_template_api_v1_admin_email_templates_key_reset_post**](EmailTemplatesApi.md#reset_template_api_v1_admin_email_templates_key_reset_post) | **POST** /api/v1/admin/email-templates/{key}/reset | Reset Template
[**reset_template_api_v1_admin_email_templates_key_reset_post_0**](EmailTemplatesApi.md#reset_template_api_v1_admin_email_templates_key_reset_post_0) | **POST** /api/v1/admin/email-templates/{key}/reset | Reset Template
[**send_test_api_v1_admin_email_templates_key_send_test_post**](EmailTemplatesApi.md#send_test_api_v1_admin_email_templates_key_send_test_post) | **POST** /api/v1/admin/email-templates/{key}/send-test | Send Test
[**send_test_api_v1_admin_email_templates_key_send_test_post_0**](EmailTemplatesApi.md#send_test_api_v1_admin_email_templates_key_send_test_post_0) | **POST** /api/v1/admin/email-templates/{key}/send-test | Send Test
[**update_template_api_v1_admin_email_templates_key_put**](EmailTemplatesApi.md#update_template_api_v1_admin_email_templates_key_put) | **PUT** /api/v1/admin/email-templates/{key} | Update Template
[**update_template_api_v1_admin_email_templates_key_put_0**](EmailTemplatesApi.md#update_template_api_v1_admin_email_templates_key_put_0) | **PUT** /api/v1/admin/email-templates/{key} | Update Template


# **get_template_api_v1_admin_email_templates_key_get**
> object get_template_api_v1_admin_email_templates_key_get(key)

Get Template

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
    api_instance = sensecore.EmailTemplatesApi(api_client)
    key = 'key_example' # str | 

    try:
        # Get Template
        api_response = api_instance.get_template_api_v1_admin_email_templates_key_get(key)
        print("The response of EmailTemplatesApi->get_template_api_v1_admin_email_templates_key_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->get_template_api_v1_admin_email_templates_key_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 

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

# **get_template_api_v1_admin_email_templates_key_get_0**
> object get_template_api_v1_admin_email_templates_key_get_0(key)

Get Template

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
    api_instance = sensecore.EmailTemplatesApi(api_client)
    key = 'key_example' # str | 

    try:
        # Get Template
        api_response = api_instance.get_template_api_v1_admin_email_templates_key_get_0(key)
        print("The response of EmailTemplatesApi->get_template_api_v1_admin_email_templates_key_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->get_template_api_v1_admin_email_templates_key_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 

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

# **list_templates_api_v1_admin_email_templates_get**
> object list_templates_api_v1_admin_email_templates_get()

List Templates

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
    api_instance = sensecore.EmailTemplatesApi(api_client)

    try:
        # List Templates
        api_response = api_instance.list_templates_api_v1_admin_email_templates_get()
        print("The response of EmailTemplatesApi->list_templates_api_v1_admin_email_templates_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->list_templates_api_v1_admin_email_templates_get: %s\n" % e)
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

# **list_templates_api_v1_admin_email_templates_get_0**
> object list_templates_api_v1_admin_email_templates_get_0()

List Templates

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
    api_instance = sensecore.EmailTemplatesApi(api_client)

    try:
        # List Templates
        api_response = api_instance.list_templates_api_v1_admin_email_templates_get_0()
        print("The response of EmailTemplatesApi->list_templates_api_v1_admin_email_templates_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->list_templates_api_v1_admin_email_templates_get_0: %s\n" % e)
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

# **preview_template_api_v1_admin_email_templates_key_preview_post**
> object preview_template_api_v1_admin_email_templates_key_preview_post(key, body=body)

Preview Template

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
    api_instance = sensecore.EmailTemplatesApi(api_client)
    key = 'key_example' # str | 
    body = None # object |  (optional)

    try:
        # Preview Template
        api_response = api_instance.preview_template_api_v1_admin_email_templates_key_preview_post(key, body=body)
        print("The response of EmailTemplatesApi->preview_template_api_v1_admin_email_templates_key_preview_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->preview_template_api_v1_admin_email_templates_key_preview_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 
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

# **preview_template_api_v1_admin_email_templates_key_preview_post_0**
> object preview_template_api_v1_admin_email_templates_key_preview_post_0(key, body=body)

Preview Template

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
    api_instance = sensecore.EmailTemplatesApi(api_client)
    key = 'key_example' # str | 
    body = None # object |  (optional)

    try:
        # Preview Template
        api_response = api_instance.preview_template_api_v1_admin_email_templates_key_preview_post_0(key, body=body)
        print("The response of EmailTemplatesApi->preview_template_api_v1_admin_email_templates_key_preview_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->preview_template_api_v1_admin_email_templates_key_preview_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 
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

# **reset_template_api_v1_admin_email_templates_key_reset_post**
> object reset_template_api_v1_admin_email_templates_key_reset_post(key)

Reset Template

For now, reset = re-run migration script for that template.
User-friendly reset is to manually paste the default and save.

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
    api_instance = sensecore.EmailTemplatesApi(api_client)
    key = 'key_example' # str | 

    try:
        # Reset Template
        api_response = api_instance.reset_template_api_v1_admin_email_templates_key_reset_post(key)
        print("The response of EmailTemplatesApi->reset_template_api_v1_admin_email_templates_key_reset_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->reset_template_api_v1_admin_email_templates_key_reset_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 

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

# **reset_template_api_v1_admin_email_templates_key_reset_post_0**
> object reset_template_api_v1_admin_email_templates_key_reset_post_0(key)

Reset Template

For now, reset = re-run migration script for that template.
User-friendly reset is to manually paste the default and save.

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
    api_instance = sensecore.EmailTemplatesApi(api_client)
    key = 'key_example' # str | 

    try:
        # Reset Template
        api_response = api_instance.reset_template_api_v1_admin_email_templates_key_reset_post_0(key)
        print("The response of EmailTemplatesApi->reset_template_api_v1_admin_email_templates_key_reset_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->reset_template_api_v1_admin_email_templates_key_reset_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 

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

# **send_test_api_v1_admin_email_templates_key_send_test_post**
> object send_test_api_v1_admin_email_templates_key_send_test_post(key, body)

Send Test

Body: {
  "to_email": "your@email",
  "provider_key": "sendgrid"  // optional. Default: active provider.
}

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
    api_instance = sensecore.EmailTemplatesApi(api_client)
    key = 'key_example' # str | 
    body = None # object | 

    try:
        # Send Test
        api_response = api_instance.send_test_api_v1_admin_email_templates_key_send_test_post(key, body)
        print("The response of EmailTemplatesApi->send_test_api_v1_admin_email_templates_key_send_test_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->send_test_api_v1_admin_email_templates_key_send_test_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 
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

# **send_test_api_v1_admin_email_templates_key_send_test_post_0**
> object send_test_api_v1_admin_email_templates_key_send_test_post_0(key, body)

Send Test

Body: {
  "to_email": "your@email",
  "provider_key": "sendgrid"  // optional. Default: active provider.
}

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
    api_instance = sensecore.EmailTemplatesApi(api_client)
    key = 'key_example' # str | 
    body = None # object | 

    try:
        # Send Test
        api_response = api_instance.send_test_api_v1_admin_email_templates_key_send_test_post_0(key, body)
        print("The response of EmailTemplatesApi->send_test_api_v1_admin_email_templates_key_send_test_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->send_test_api_v1_admin_email_templates_key_send_test_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 
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

# **update_template_api_v1_admin_email_templates_key_put**
> object update_template_api_v1_admin_email_templates_key_put(key, body)

Update Template

Body: {
  "subject", "body_markdown", "button_label", "button_link",
  "is_enabled" (bool), "note" (optional)
}

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
    api_instance = sensecore.EmailTemplatesApi(api_client)
    key = 'key_example' # str | 
    body = None # object | 

    try:
        # Update Template
        api_response = api_instance.update_template_api_v1_admin_email_templates_key_put(key, body)
        print("The response of EmailTemplatesApi->update_template_api_v1_admin_email_templates_key_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->update_template_api_v1_admin_email_templates_key_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 
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

# **update_template_api_v1_admin_email_templates_key_put_0**
> object update_template_api_v1_admin_email_templates_key_put_0(key, body)

Update Template

Body: {
  "subject", "body_markdown", "button_label", "button_link",
  "is_enabled" (bool), "note" (optional)
}

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
    api_instance = sensecore.EmailTemplatesApi(api_client)
    key = 'key_example' # str | 
    body = None # object | 

    try:
        # Update Template
        api_response = api_instance.update_template_api_v1_admin_email_templates_key_put_0(key, body)
        print("The response of EmailTemplatesApi->update_template_api_v1_admin_email_templates_key_put_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EmailTemplatesApi->update_template_api_v1_admin_email_templates_key_put_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **str**|  | 
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

