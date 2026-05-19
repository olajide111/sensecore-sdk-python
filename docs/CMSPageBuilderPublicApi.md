# sensecore.CMSPageBuilderPublicApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**public_list_sections_api_v1_cms_page_sections_page_get**](CMSPageBuilderPublicApi.md#public_list_sections_api_v1_cms_page_sections_page_get) | **GET** /api/v1/cms/page-sections/{page} | Public List Sections
[**public_list_sections_api_v1_cms_page_sections_page_get_0**](CMSPageBuilderPublicApi.md#public_list_sections_api_v1_cms_page_sections_page_get_0) | **GET** /api/v1/cms/page-sections/{page} | Public List Sections


# **public_list_sections_api_v1_cms_page_sections_page_get**
> object public_list_sections_api_v1_cms_page_sections_page_get(page)

Public List Sections

Public list of published sections for a page, ordered by sort_order.

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
    api_instance = sensecore.CMSPageBuilderPublicApi(api_client)
    page = 'page_example' # str | 

    try:
        # Public List Sections
        api_response = api_instance.public_list_sections_api_v1_cms_page_sections_page_get(page)
        print("The response of CMSPageBuilderPublicApi->public_list_sections_api_v1_cms_page_sections_page_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPageBuilderPublicApi->public_list_sections_api_v1_cms_page_sections_page_get: %s\n" % e)
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

# **public_list_sections_api_v1_cms_page_sections_page_get_0**
> object public_list_sections_api_v1_cms_page_sections_page_get_0(page)

Public List Sections

Public list of published sections for a page, ordered by sort_order.

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
    api_instance = sensecore.CMSPageBuilderPublicApi(api_client)
    page = 'page_example' # str | 

    try:
        # Public List Sections
        api_response = api_instance.public_list_sections_api_v1_cms_page_sections_page_get_0(page)
        print("The response of CMSPageBuilderPublicApi->public_list_sections_api_v1_cms_page_sections_page_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CMSPageBuilderPublicApi->public_list_sections_api_v1_cms_page_sections_page_get_0: %s\n" % e)
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

