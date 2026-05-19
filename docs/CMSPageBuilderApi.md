# sensecore.CMSPageBuilderApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_section_api_v1_admin_cms_pages_builder_page_sections_post**](CMSPageBuilderApi.md#add_section_api_v1_admin_cms_pages_builder_page_sections_post) | **POST** /api/v1/admin/cms/pages-builder/{page}/sections | Add Section
[**add_section_api_v1_admin_cms_pages_builder_page_sections_post_0**](CMSPageBuilderApi.md#add_section_api_v1_admin_cms_pages_builder_page_sections_post_0) | **POST** /api/v1/admin/cms/pages-builder/{page}/sections | Add Section
[**list_sections_api_v1_admin_cms_pages_builder_page_sections_get**](CMSPageBuilderApi.md#list_sections_api_v1_admin_cms_pages_builder_page_sections_get) | **GET** /api/v1/admin/cms/pages-builder/{page}/sections | List Sections
[**list_sections_api_v1_admin_cms_pages_builder_page_sections_get_0**](CMSPageBuilderApi.md#list_sections_api_v1_admin_cms_pages_builder_page_sections_get_0) | **GET** /api/v1/admin/cms/pages-builder/{page}/sections | List Sections
[**reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put**](CMSPageBuilderApi.md#reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put) | **PUT** /api/v1/admin/cms/pages-builder/{page}/reorder | Reorder Sections
[**reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put_0**](CMSPageBuilderApi.md#reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put_0) | **PUT** /api/v1/admin/cms/pages-builder/{page}/reorder | Reorder Sections


# **add_section_api_v1_admin_cms_pages_builder_page_sections_post**
> object add_section_api_v1_admin_cms_pages_builder_page_sections_post(page, body)

Add Section

Body:
  {
    "section":      "hero_v2",   (required, unique per page)
    "section_type": "hero",      (required, picks the editor in admin)
    "content":      {...},        (optional, default {})
    "title":        "Hero v2",   (optional, friendly label)
    "is_published": true,         (optional, default true)
    "sort_order":   null          (optional, default = max+1)
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
    api_instance = sensecore.CMSPageBuilderApi(api_client)
    page = 'page_example' # str | 
    body = None # object | 

    try:
        # Add Section
        api_response = api_instance.add_section_api_v1_admin_cms_pages_builder_page_sections_post(page, body)
        print("The response of CMSPageBuilderApi->add_section_api_v1_admin_cms_pages_builder_page_sections_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPageBuilderApi->add_section_api_v1_admin_cms_pages_builder_page_sections_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **str**|  | 
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

# **add_section_api_v1_admin_cms_pages_builder_page_sections_post_0**
> object add_section_api_v1_admin_cms_pages_builder_page_sections_post_0(page, body)

Add Section

Body:
  {
    "section":      "hero_v2",   (required, unique per page)
    "section_type": "hero",      (required, picks the editor in admin)
    "content":      {...},        (optional, default {})
    "title":        "Hero v2",   (optional, friendly label)
    "is_published": true,         (optional, default true)
    "sort_order":   null          (optional, default = max+1)
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
    api_instance = sensecore.CMSPageBuilderApi(api_client)
    page = 'page_example' # str | 
    body = None # object | 

    try:
        # Add Section
        api_response = api_instance.add_section_api_v1_admin_cms_pages_builder_page_sections_post_0(page, body)
        print("The response of CMSPageBuilderApi->add_section_api_v1_admin_cms_pages_builder_page_sections_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPageBuilderApi->add_section_api_v1_admin_cms_pages_builder_page_sections_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **str**|  | 
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

# **list_sections_api_v1_admin_cms_pages_builder_page_sections_get**
> object list_sections_api_v1_admin_cms_pages_builder_page_sections_get(page)

List Sections

Return all sections for a page, ordered by sort_order.

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
    api_instance = sensecore.CMSPageBuilderApi(api_client)
    page = 'page_example' # str | 

    try:
        # List Sections
        api_response = api_instance.list_sections_api_v1_admin_cms_pages_builder_page_sections_get(page)
        print("The response of CMSPageBuilderApi->list_sections_api_v1_admin_cms_pages_builder_page_sections_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPageBuilderApi->list_sections_api_v1_admin_cms_pages_builder_page_sections_get: %s\n" % e)
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

# **list_sections_api_v1_admin_cms_pages_builder_page_sections_get_0**
> object list_sections_api_v1_admin_cms_pages_builder_page_sections_get_0(page)

List Sections

Return all sections for a page, ordered by sort_order.

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
    api_instance = sensecore.CMSPageBuilderApi(api_client)
    page = 'page_example' # str | 

    try:
        # List Sections
        api_response = api_instance.list_sections_api_v1_admin_cms_pages_builder_page_sections_get_0(page)
        print("The response of CMSPageBuilderApi->list_sections_api_v1_admin_cms_pages_builder_page_sections_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPageBuilderApi->list_sections_api_v1_admin_cms_pages_builder_page_sections_get_0: %s\n" % e)
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

# **reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put**
> object reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put(page, body)

Reorder Sections

Body: { "order": ["hero", "stats", "cta", ...] }
Position in the array becomes the new sort_order (0-indexed).
Sections not listed are left alone.

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
    api_instance = sensecore.CMSPageBuilderApi(api_client)
    page = 'page_example' # str | 
    body = None # object | 

    try:
        # Reorder Sections
        api_response = api_instance.reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put(page, body)
        print("The response of CMSPageBuilderApi->reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPageBuilderApi->reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **str**|  | 
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

# **reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put_0**
> object reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put_0(page, body)

Reorder Sections

Body: { "order": ["hero", "stats", "cta", ...] }
Position in the array becomes the new sort_order (0-indexed).
Sections not listed are left alone.

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
    api_instance = sensecore.CMSPageBuilderApi(api_client)
    page = 'page_example' # str | 
    body = None # object | 

    try:
        # Reorder Sections
        api_response = api_instance.reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put_0(page, body)
        print("The response of CMSPageBuilderApi->reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPageBuilderApi->reorder_sections_api_v1_admin_cms_pages_builder_page_reorder_put_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **str**|  | 
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

