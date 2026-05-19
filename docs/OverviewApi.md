# sensecore.OverviewApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_overview_api_v1_overview_dashboard_get**](OverviewApi.md#get_overview_api_v1_overview_dashboard_get) | **GET** /api/v1/overview/dashboard | Get Overview
[**get_overview_api_v1_overview_dashboard_get_0**](OverviewApi.md#get_overview_api_v1_overview_dashboard_get_0) | **GET** /api/v1/overview/dashboard | Get Overview


# **get_overview_api_v1_overview_dashboard_get**
> object get_overview_api_v1_overview_dashboard_get()

Get Overview

Returns overview dashboard data.
Real data from DB when available, demo fallback when not.

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
    api_instance = sensecore.OverviewApi(api_client)

    try:
        # Get Overview
        api_response = api_instance.get_overview_api_v1_overview_dashboard_get()
        print("The response of OverviewApi->get_overview_api_v1_overview_dashboard_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OverviewApi->get_overview_api_v1_overview_dashboard_get: %s\n" % e)
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

# **get_overview_api_v1_overview_dashboard_get_0**
> object get_overview_api_v1_overview_dashboard_get_0()

Get Overview

Returns overview dashboard data.
Real data from DB when available, demo fallback when not.

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
    api_instance = sensecore.OverviewApi(api_client)

    try:
        # Get Overview
        api_response = api_instance.get_overview_api_v1_overview_dashboard_get_0()
        print("The response of OverviewApi->get_overview_api_v1_overview_dashboard_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OverviewApi->get_overview_api_v1_overview_dashboard_get_0: %s\n" % e)
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

