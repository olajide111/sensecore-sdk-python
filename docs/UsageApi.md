# sensecore.UsageApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get**](UsageApi.md#admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get) | **GET** /api/v1/usage/admin/org/{org_id} | Admin Org Detail Endpoint
[**admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get_0**](UsageApi.md#admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get_0) | **GET** /api/v1/usage/admin/org/{org_id} | Admin Org Detail Endpoint
[**admin_overview_endpoint_api_v1_usage_admin_overview_get**](UsageApi.md#admin_overview_endpoint_api_v1_usage_admin_overview_get) | **GET** /api/v1/usage/admin/overview | Admin Overview Endpoint
[**admin_overview_endpoint_api_v1_usage_admin_overview_get_0**](UsageApi.md#admin_overview_endpoint_api_v1_usage_admin_overview_get_0) | **GET** /api/v1/usage/admin/overview | Admin Overview Endpoint
[**my_history_endpoint_api_v1_usage_me_history_get**](UsageApi.md#my_history_endpoint_api_v1_usage_me_history_get) | **GET** /api/v1/usage/me/history | My History Endpoint
[**my_history_endpoint_api_v1_usage_me_history_get_0**](UsageApi.md#my_history_endpoint_api_v1_usage_me_history_get_0) | **GET** /api/v1/usage/me/history | My History Endpoint
[**my_usage_endpoint_api_v1_usage_me_get**](UsageApi.md#my_usage_endpoint_api_v1_usage_me_get) | **GET** /api/v1/usage/me | My Usage Endpoint
[**my_usage_endpoint_api_v1_usage_me_get_0**](UsageApi.md#my_usage_endpoint_api_v1_usage_me_get_0) | **GET** /api/v1/usage/me | My Usage Endpoint


# **admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get**
> object admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get(org_id)

Admin Org Detail Endpoint

Drill-down on any single organisation. Returns the same shape
as /me plus the org's display name and 30-day history.

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
    api_instance = sensecore.UsageApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Admin Org Detail Endpoint
        api_response = api_instance.admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get(org_id)
        print("The response of UsageApi->admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsageApi->admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**|  | 

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
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get_0**
> object admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get_0(org_id)

Admin Org Detail Endpoint

Drill-down on any single organisation. Returns the same shape
as /me plus the org's display name and 30-day history.

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
    api_instance = sensecore.UsageApi(api_client)
    org_id = 'org_id_example' # str | 

    try:
        # Admin Org Detail Endpoint
        api_response = api_instance.admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get_0(org_id)
        print("The response of UsageApi->admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsageApi->admin_org_detail_endpoint_api_v1_usage_admin_org_org_id_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **str**|  | 

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
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **admin_overview_endpoint_api_v1_usage_admin_overview_get**
> object admin_overview_endpoint_api_v1_usage_admin_overview_get()

Admin Overview Endpoint

All-orgs roll-up. Aggregate KPIs filtered to attributed traffic
only (excludes unauthenticated noise) + per-org table with status
flags (ok / warning / over).

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
    api_instance = sensecore.UsageApi(api_client)

    try:
        # Admin Overview Endpoint
        api_response = api_instance.admin_overview_endpoint_api_v1_usage_admin_overview_get()
        print("The response of UsageApi->admin_overview_endpoint_api_v1_usage_admin_overview_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsageApi->admin_overview_endpoint_api_v1_usage_admin_overview_get: %s\n" % e)
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

# **admin_overview_endpoint_api_v1_usage_admin_overview_get_0**
> object admin_overview_endpoint_api_v1_usage_admin_overview_get_0()

Admin Overview Endpoint

All-orgs roll-up. Aggregate KPIs filtered to attributed traffic
only (excludes unauthenticated noise) + per-org table with status
flags (ok / warning / over).

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
    api_instance = sensecore.UsageApi(api_client)

    try:
        # Admin Overview Endpoint
        api_response = api_instance.admin_overview_endpoint_api_v1_usage_admin_overview_get_0()
        print("The response of UsageApi->admin_overview_endpoint_api_v1_usage_admin_overview_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsageApi->admin_overview_endpoint_api_v1_usage_admin_overview_get_0: %s\n" % e)
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

# **my_history_endpoint_api_v1_usage_me_history_get**
> object my_history_endpoint_api_v1_usage_me_history_get(days=days, x_api_key=x_api_key)

My History Endpoint

Daily call counts for the last N days (1-90), zero-filled.

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
    api_instance = sensecore.UsageApi(api_client)
    days = 30 # int |  (optional) (default to 30)
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # My History Endpoint
        api_response = api_instance.my_history_endpoint_api_v1_usage_me_history_get(days=days, x_api_key=x_api_key)
        print("The response of UsageApi->my_history_endpoint_api_v1_usage_me_history_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsageApi->my_history_endpoint_api_v1_usage_me_history_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **days** | **int**|  | [optional] [default to 30]
 **x_api_key** | **str**|  | [optional] 

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
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **my_history_endpoint_api_v1_usage_me_history_get_0**
> object my_history_endpoint_api_v1_usage_me_history_get_0(days=days, x_api_key=x_api_key)

My History Endpoint

Daily call counts for the last N days (1-90), zero-filled.

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
    api_instance = sensecore.UsageApi(api_client)
    days = 30 # int |  (optional) (default to 30)
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # My History Endpoint
        api_response = api_instance.my_history_endpoint_api_v1_usage_me_history_get_0(days=days, x_api_key=x_api_key)
        print("The response of UsageApi->my_history_endpoint_api_v1_usage_me_history_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsageApi->my_history_endpoint_api_v1_usage_me_history_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **days** | **int**|  | [optional] [default to 30]
 **x_api_key** | **str**|  | [optional] 

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
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **my_usage_endpoint_api_v1_usage_me_get**
> object my_usage_endpoint_api_v1_usage_me_get(x_api_key=x_api_key)

My Usage Endpoint

Current calendar-month usage summary for the caller's organisation.

Returns plan_key, max_api_calls (None if unlimited), calls_this_month,
percent_used, calls_today, error_rate_pct, p95_latency_ms, and the
top 10 endpoints this month.

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
    api_instance = sensecore.UsageApi(api_client)
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # My Usage Endpoint
        api_response = api_instance.my_usage_endpoint_api_v1_usage_me_get(x_api_key=x_api_key)
        print("The response of UsageApi->my_usage_endpoint_api_v1_usage_me_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsageApi->my_usage_endpoint_api_v1_usage_me_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_api_key** | **str**|  | [optional] 

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
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **my_usage_endpoint_api_v1_usage_me_get_0**
> object my_usage_endpoint_api_v1_usage_me_get_0(x_api_key=x_api_key)

My Usage Endpoint

Current calendar-month usage summary for the caller's organisation.

Returns plan_key, max_api_calls (None if unlimited), calls_this_month,
percent_used, calls_today, error_rate_pct, p95_latency_ms, and the
top 10 endpoints this month.

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
    api_instance = sensecore.UsageApi(api_client)
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # My Usage Endpoint
        api_response = api_instance.my_usage_endpoint_api_v1_usage_me_get_0(x_api_key=x_api_key)
        print("The response of UsageApi->my_usage_endpoint_api_v1_usage_me_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsageApi->my_usage_endpoint_api_v1_usage_me_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **x_api_key** | **str**|  | [optional] 

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
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

