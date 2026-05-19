# sensecore.PublicApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_public_invoice_api_v1_invoice_public_token_get**](PublicApi.md#get_public_invoice_api_v1_invoice_public_token_get) | **GET** /api/v1/invoice/public/{token} | Get Public Invoice


# **get_public_invoice_api_v1_invoice_public_token_get**
> object get_public_invoice_api_v1_invoice_public_token_get(token)

Get Public Invoice

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
    api_instance = sensecore.PublicApi(api_client)
    token = 'token_example' # str | 

    try:
        # Get Public Invoice
        api_response = api_instance.get_public_invoice_api_v1_invoice_public_token_get(token)
        print("The response of PublicApi->get_public_invoice_api_v1_invoice_public_token_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PublicApi->get_public_invoice_api_v1_invoice_public_token_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **str**|  | 

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

