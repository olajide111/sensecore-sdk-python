# sensecore.CMSPublicApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**public_announcement_api_v1_cms_announcement_get**](CMSPublicApi.md#public_announcement_api_v1_cms_announcement_get) | **GET** /api/v1/cms/announcement | Public Announcement
[**public_announcement_api_v1_cms_announcement_get_0**](CMSPublicApi.md#public_announcement_api_v1_cms_announcement_get_0) | **GET** /api/v1/cms/announcement | Public Announcement
[**public_asset_api_v1_cms_asset_aid_get**](CMSPublicApi.md#public_asset_api_v1_cms_asset_aid_get) | **GET** /api/v1/cms/asset/{aid} | Public Asset
[**public_asset_api_v1_cms_asset_aid_get_0**](CMSPublicApi.md#public_asset_api_v1_cms_asset_aid_get_0) | **GET** /api/v1/cms/asset/{aid} | Public Asset
[**public_blog_get_api_v1_cms_blog_slug_get**](CMSPublicApi.md#public_blog_get_api_v1_cms_blog_slug_get) | **GET** /api/v1/cms/blog/{slug} | Public Blog Get
[**public_blog_get_api_v1_cms_blog_slug_get_0**](CMSPublicApi.md#public_blog_get_api_v1_cms_blog_slug_get_0) | **GET** /api/v1/cms/blog/{slug} | Public Blog Get
[**public_blog_list_api_v1_cms_blog_get**](CMSPublicApi.md#public_blog_list_api_v1_cms_blog_get) | **GET** /api/v1/cms/blog | Public Blog List
[**public_blog_list_api_v1_cms_blog_get_0**](CMSPublicApi.md#public_blog_list_api_v1_cms_blog_get_0) | **GET** /api/v1/cms/blog | Public Blog List
[**public_branding_api_v1_cms_branding_get**](CMSPublicApi.md#public_branding_api_v1_cms_branding_get) | **GET** /api/v1/cms/branding | Public Branding
[**public_branding_api_v1_cms_branding_get_0**](CMSPublicApi.md#public_branding_api_v1_cms_branding_get_0) | **GET** /api/v1/cms/branding | Public Branding
[**public_changelog_api_v1_cms_changelog_get**](CMSPublicApi.md#public_changelog_api_v1_cms_changelog_get) | **GET** /api/v1/cms/changelog | Public Changelog
[**public_changelog_api_v1_cms_changelog_get_0**](CMSPublicApi.md#public_changelog_api_v1_cms_changelog_get_0) | **GET** /api/v1/cms/changelog | Public Changelog
[**public_get_page_api_v1_cms_content_page_get**](CMSPublicApi.md#public_get_page_api_v1_cms_content_page_get) | **GET** /api/v1/cms/content/{page} | Public Get Page
[**public_get_page_api_v1_cms_content_page_get_0**](CMSPublicApi.md#public_get_page_api_v1_cms_content_page_get_0) | **GET** /api/v1/cms/content/{page} | Public Get Page


# **public_announcement_api_v1_cms_announcement_get**
> object public_announcement_api_v1_cms_announcement_get()

Public Announcement

Public announcement banner.

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
    api_instance = sensecore.CMSPublicApi(api_client)

    try:
        # Public Announcement
        api_response = api_instance.public_announcement_api_v1_cms_announcement_get()
        print("The response of CMSPublicApi->public_announcement_api_v1_cms_announcement_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_announcement_api_v1_cms_announcement_get: %s\n" % e)
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

# **public_announcement_api_v1_cms_announcement_get_0**
> object public_announcement_api_v1_cms_announcement_get_0()

Public Announcement

Public announcement banner.

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
    api_instance = sensecore.CMSPublicApi(api_client)

    try:
        # Public Announcement
        api_response = api_instance.public_announcement_api_v1_cms_announcement_get_0()
        print("The response of CMSPublicApi->public_announcement_api_v1_cms_announcement_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_announcement_api_v1_cms_announcement_get_0: %s\n" % e)
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

# **public_asset_api_v1_cms_asset_aid_get**
> object public_asset_api_v1_cms_asset_aid_get(aid)

Public Asset

Stream asset binary.

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
    api_instance = sensecore.CMSPublicApi(api_client)
    aid = 'aid_example' # str | 

    try:
        # Public Asset
        api_response = api_instance.public_asset_api_v1_cms_asset_aid_get(aid)
        print("The response of CMSPublicApi->public_asset_api_v1_cms_asset_aid_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_asset_api_v1_cms_asset_aid_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **aid** | **str**|  | 

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

# **public_asset_api_v1_cms_asset_aid_get_0**
> object public_asset_api_v1_cms_asset_aid_get_0(aid)

Public Asset

Stream asset binary.

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
    api_instance = sensecore.CMSPublicApi(api_client)
    aid = 'aid_example' # str | 

    try:
        # Public Asset
        api_response = api_instance.public_asset_api_v1_cms_asset_aid_get_0(aid)
        print("The response of CMSPublicApi->public_asset_api_v1_cms_asset_aid_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_asset_api_v1_cms_asset_aid_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **aid** | **str**|  | 

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

# **public_blog_get_api_v1_cms_blog_slug_get**
> object public_blog_get_api_v1_cms_blog_slug_get(slug)

Public Blog Get

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
    api_instance = sensecore.CMSPublicApi(api_client)
    slug = 'slug_example' # str | 

    try:
        # Public Blog Get
        api_response = api_instance.public_blog_get_api_v1_cms_blog_slug_get(slug)
        print("The response of CMSPublicApi->public_blog_get_api_v1_cms_blog_slug_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_blog_get_api_v1_cms_blog_slug_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **str**|  | 

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

# **public_blog_get_api_v1_cms_blog_slug_get_0**
> object public_blog_get_api_v1_cms_blog_slug_get_0(slug)

Public Blog Get

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
    api_instance = sensecore.CMSPublicApi(api_client)
    slug = 'slug_example' # str | 

    try:
        # Public Blog Get
        api_response = api_instance.public_blog_get_api_v1_cms_blog_slug_get_0(slug)
        print("The response of CMSPublicApi->public_blog_get_api_v1_cms_blog_slug_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_blog_get_api_v1_cms_blog_slug_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **str**|  | 

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

# **public_blog_list_api_v1_cms_blog_get**
> object public_blog_list_api_v1_cms_blog_get()

Public Blog List

Public blog list.

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
    api_instance = sensecore.CMSPublicApi(api_client)

    try:
        # Public Blog List
        api_response = api_instance.public_blog_list_api_v1_cms_blog_get()
        print("The response of CMSPublicApi->public_blog_list_api_v1_cms_blog_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_blog_list_api_v1_cms_blog_get: %s\n" % e)
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

# **public_blog_list_api_v1_cms_blog_get_0**
> object public_blog_list_api_v1_cms_blog_get_0()

Public Blog List

Public blog list.

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
    api_instance = sensecore.CMSPublicApi(api_client)

    try:
        # Public Blog List
        api_response = api_instance.public_blog_list_api_v1_cms_blog_get_0()
        print("The response of CMSPublicApi->public_blog_list_api_v1_cms_blog_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_blog_list_api_v1_cms_blog_get_0: %s\n" % e)
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

# **public_branding_api_v1_cms_branding_get**
> object public_branding_api_v1_cms_branding_get()

Public Branding

Public branding for marketing site.

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
    api_instance = sensecore.CMSPublicApi(api_client)

    try:
        # Public Branding
        api_response = api_instance.public_branding_api_v1_cms_branding_get()
        print("The response of CMSPublicApi->public_branding_api_v1_cms_branding_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_branding_api_v1_cms_branding_get: %s\n" % e)
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

# **public_branding_api_v1_cms_branding_get_0**
> object public_branding_api_v1_cms_branding_get_0()

Public Branding

Public branding for marketing site.

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
    api_instance = sensecore.CMSPublicApi(api_client)

    try:
        # Public Branding
        api_response = api_instance.public_branding_api_v1_cms_branding_get_0()
        print("The response of CMSPublicApi->public_branding_api_v1_cms_branding_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_branding_api_v1_cms_branding_get_0: %s\n" % e)
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

# **public_changelog_api_v1_cms_changelog_get**
> object public_changelog_api_v1_cms_changelog_get()

Public Changelog

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
    api_instance = sensecore.CMSPublicApi(api_client)

    try:
        # Public Changelog
        api_response = api_instance.public_changelog_api_v1_cms_changelog_get()
        print("The response of CMSPublicApi->public_changelog_api_v1_cms_changelog_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_changelog_api_v1_cms_changelog_get: %s\n" % e)
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

# **public_changelog_api_v1_cms_changelog_get_0**
> object public_changelog_api_v1_cms_changelog_get_0()

Public Changelog

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
    api_instance = sensecore.CMSPublicApi(api_client)

    try:
        # Public Changelog
        api_response = api_instance.public_changelog_api_v1_cms_changelog_get_0()
        print("The response of CMSPublicApi->public_changelog_api_v1_cms_changelog_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_changelog_api_v1_cms_changelog_get_0: %s\n" % e)
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

# **public_get_page_api_v1_cms_content_page_get**
> object public_get_page_api_v1_cms_content_page_get(page)

Public Get Page

Public endpoint for marketing site to fetch published content.

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
    api_instance = sensecore.CMSPublicApi(api_client)
    page = 'page_example' # str | 

    try:
        # Public Get Page
        api_response = api_instance.public_get_page_api_v1_cms_content_page_get(page)
        print("The response of CMSPublicApi->public_get_page_api_v1_cms_content_page_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_get_page_api_v1_cms_content_page_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **str**|  | 

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

# **public_get_page_api_v1_cms_content_page_get_0**
> object public_get_page_api_v1_cms_content_page_get_0(page)

Public Get Page

Public endpoint for marketing site to fetch published content.

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
    api_instance = sensecore.CMSPublicApi(api_client)
    page = 'page_example' # str | 

    try:
        # Public Get Page
        api_response = api_instance.public_get_page_api_v1_cms_content_page_get_0(page)
        print("The response of CMSPublicApi->public_get_page_api_v1_cms_content_page_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPublicApi->public_get_page_api_v1_cms_content_page_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **str**|  | 

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

