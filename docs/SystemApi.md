# sensecore.SystemApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**health_api_v1_health_head**](SystemApi.md#health_api_v1_health_head) | **GET** /api/v1/health | Health
[**health_api_v1_health_head_0**](SystemApi.md#health_api_v1_health_head_0) | **HEAD** /api/v1/health | Health


# **health_api_v1_health_head**
> HealthResponse health_api_v1_health_head()

Health

Returns API status, DB connectivity, loaded models, and uptime. No authentication required.

### Example


```python
import sensecore
from sensecore.models.health_response import HealthResponse
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
    api_instance = sensecore.SystemApi(api_client)

    try:
        # Health
        api_response = api_instance.health_api_v1_health_head()
        print("The response of SystemApi->health_api_v1_health_head:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemApi->health_api_v1_health_head: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**HealthResponse**](HealthResponse.md)

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

# **health_api_v1_health_head_0**
> HealthResponse health_api_v1_health_head_0()

Health

Returns API status, DB connectivity, loaded models, and uptime. No authentication required.

### Example


```python
import sensecore
from sensecore.models.health_response import HealthResponse
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
    api_instance = sensecore.SystemApi(api_client)

    try:
        # Health
        api_response = api_instance.health_api_v1_health_head_0()
        print("The response of SystemApi->health_api_v1_health_head_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SystemApi->health_api_v1_health_head_0: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**HealthResponse**](HealthResponse.md)

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

