# sensecore.AdminClientHealthApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_client_health_api_v1_admin_client_health_get**](AdminClientHealthApi.md#get_client_health_api_v1_admin_client_health_get) | **GET** /api/v1/admin/client-health | Get Client Health


# **get_client_health_api_v1_admin_client_health_get**
> object get_client_health_api_v1_admin_client_health_get()

Get Client Health

Single endpoint returning all 7 sections of the Client Health dashboard.

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
    api_instance = sensecore.AdminClientHealthApi(api_client)

    try:
        # Get Client Health
        api_response = api_instance.get_client_health_api_v1_admin_client_health_get()
        print("The response of AdminClientHealthApi->get_client_health_api_v1_admin_client_health_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AdminClientHealthApi->get_client_health_api_v1_admin_client_health_get: %s\n" % e)
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

