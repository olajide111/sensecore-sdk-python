# sensecore.MetersApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**list_meters_api_v1_meters_get**](MetersApi.md#list_meters_api_v1_meters_get) | **GET** /api/v1/meters | List Meters


# **list_meters_api_v1_meters_get**
> object list_meters_api_v1_meters_get()

List Meters

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
    api_instance = sensecore.MetersApi(api_client)

    try:
        # List Meters
        api_response = api_instance.list_meters_api_v1_meters_get()
        print("The response of MetersApi->list_meters_api_v1_meters_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MetersApi->list_meters_api_v1_meters_get: %s\n" % e)
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

