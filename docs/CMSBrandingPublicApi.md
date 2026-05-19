# sensecore.CMSBrandingPublicApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_branding_full_api_v1_cms_branding_full_get**](CMSBrandingPublicApi.md#get_branding_full_api_v1_cms_branding_full_get) | **GET** /api/v1/cms/branding-full | Get Branding Full
[**get_branding_full_api_v1_cms_branding_full_get_0**](CMSBrandingPublicApi.md#get_branding_full_api_v1_cms_branding_full_get_0) | **GET** /api/v1/cms/branding-full | Get Branding Full
[**serve_favicon_api_v1_cms_favicon_get**](CMSBrandingPublicApi.md#serve_favicon_api_v1_cms_favicon_get) | **GET** /api/v1/cms/favicon | Serve Favicon
[**serve_favicon_api_v1_cms_favicon_get_0**](CMSBrandingPublicApi.md#serve_favicon_api_v1_cms_favicon_get_0) | **GET** /api/v1/cms/favicon | Serve Favicon


# **get_branding_full_api_v1_cms_branding_full_get**
> object get_branding_full_api_v1_cms_branding_full_get()

Get Branding Full

Return full branding object. Public, cacheable.

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
    api_instance = sensecore.CMSBrandingPublicApi(api_client)

    try:
        # Get Branding Full
        api_response = api_instance.get_branding_full_api_v1_cms_branding_full_get()
        print("The response of CMSBrandingPublicApi->get_branding_full_api_v1_cms_branding_full_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSBrandingPublicApi->get_branding_full_api_v1_cms_branding_full_get: %s\n" % e)
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

# **get_branding_full_api_v1_cms_branding_full_get_0**
> object get_branding_full_api_v1_cms_branding_full_get_0()

Get Branding Full

Return full branding object. Public, cacheable.

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
    api_instance = sensecore.CMSBrandingPublicApi(api_client)

    try:
        # Get Branding Full
        api_response = api_instance.get_branding_full_api_v1_cms_branding_full_get_0()
        print("The response of CMSBrandingPublicApi->get_branding_full_api_v1_cms_branding_full_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSBrandingPublicApi->get_branding_full_api_v1_cms_branding_full_get_0: %s\n" % e)
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

# **serve_favicon_api_v1_cms_favicon_get**
> object serve_favicon_api_v1_cms_favicon_get()

Serve Favicon

Redirect to configured favicon URL or fallback to /favicon.png.

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
    api_instance = sensecore.CMSBrandingPublicApi(api_client)

    try:
        # Serve Favicon
        api_response = api_instance.serve_favicon_api_v1_cms_favicon_get()
        print("The response of CMSBrandingPublicApi->serve_favicon_api_v1_cms_favicon_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSBrandingPublicApi->serve_favicon_api_v1_cms_favicon_get: %s\n" % e)
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

# **serve_favicon_api_v1_cms_favicon_get_0**
> object serve_favicon_api_v1_cms_favicon_get_0()

Serve Favicon

Redirect to configured favicon URL or fallback to /favicon.png.

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
    api_instance = sensecore.CMSBrandingPublicApi(api_client)

    try:
        # Serve Favicon
        api_response = api_instance.serve_favicon_api_v1_cms_favicon_get_0()
        print("The response of CMSBrandingPublicApi->serve_favicon_api_v1_cms_favicon_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSBrandingPublicApi->serve_favicon_api_v1_cms_favicon_get_0: %s\n" % e)
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

