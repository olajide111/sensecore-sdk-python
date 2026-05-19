# sensecore.ReadingsApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_readings_api_v1_readings_get**](ReadingsApi.md#get_readings_api_v1_readings_get) | **GET** /api/v1/readings | Get Readings
[**get_readings_api_v1_readings_meter_id_get**](ReadingsApi.md#get_readings_api_v1_readings_meter_id_get) | **GET** /api/v1/readings/{meter_id} | Get Readings
[**list_meters_api_v1_buildings_meters_get**](ReadingsApi.md#list_meters_api_v1_buildings_meters_get) | **GET** /api/v1/buildings/meters | List Meters
[**manual_reading_api_v1_readings_manual_post**](ReadingsApi.md#manual_reading_api_v1_readings_manual_post) | **POST** /api/v1/readings/manual | Manual Reading
[**push_readings_api_v1_readings_push_post**](ReadingsApi.md#push_readings_api_v1_readings_push_post) | **POST** /api/v1/readings/push | Push Readings


# **get_readings_api_v1_readings_get**
> object get_readings_api_v1_readings_get(meter_id)

Get Readings

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
    api_instance = sensecore.ReadingsApi(api_client)
    meter_id = 'meter_id_example' # str | 

    try:
        # Get Readings
        api_response = api_instance.get_readings_api_v1_readings_get(meter_id)
        print("The response of ReadingsApi->get_readings_api_v1_readings_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReadingsApi->get_readings_api_v1_readings_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **meter_id** | **str**|  | 

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

# **get_readings_api_v1_readings_meter_id_get**
> object get_readings_api_v1_readings_meter_id_get(meter_id, limit=limit)

Get Readings

Fetch the most recent readings for a meter.
Returns readings sorted by timestamp (newest first, then reversed for chart display).

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
    api_instance = sensecore.ReadingsApi(api_client)
    meter_id = 'meter_id_example' # str | 
    limit = 336 # int |  (optional) (default to 336)

    try:
        # Get Readings
        api_response = api_instance.get_readings_api_v1_readings_meter_id_get(meter_id, limit=limit)
        print("The response of ReadingsApi->get_readings_api_v1_readings_meter_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReadingsApi->get_readings_api_v1_readings_meter_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **meter_id** | **str**|  | 
 **limit** | **int**|  | [optional] [default to 336]

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

# **list_meters_api_v1_buildings_meters_get**
> object list_meters_api_v1_buildings_meters_get()

List Meters

List all meters that have ingested readings.
Returns meter_id, building name, reading count, date range, quality.

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
    api_instance = sensecore.ReadingsApi(api_client)

    try:
        # List Meters
        api_response = api_instance.list_meters_api_v1_buildings_meters_get()
        print("The response of ReadingsApi->list_meters_api_v1_buildings_meters_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReadingsApi->list_meters_api_v1_buildings_meters_get: %s\n" % e)
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

# **manual_reading_api_v1_readings_manual_post**
> ManualResponse manual_reading_api_v1_readings_manual_post(manual_request)

Manual Reading

Submit a single meter reading manually.
Used for gap-filling, testing, or manual data entry from the dashboard.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.manual_request import ManualRequest
from sensecore.models.manual_response import ManualResponse
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
    api_instance = sensecore.ReadingsApi(api_client)
    manual_request = sensecore.ManualRequest() # ManualRequest | 

    try:
        # Manual Reading
        api_response = api_instance.manual_reading_api_v1_readings_manual_post(manual_request)
        print("The response of ReadingsApi->manual_reading_api_v1_readings_manual_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReadingsApi->manual_reading_api_v1_readings_manual_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **manual_request** | [**ManualRequest**](ManualRequest.md)|  | 

### Return type

[**ManualResponse**](ManualResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **push_readings_api_v1_readings_push_post**
> PushResponse push_readings_api_v1_readings_push_post(push_request)

Push Readings

Bulk push meter readings as JSON.
Used by IoT gateways, BMS integrations, and automated data feeds.
Duplicate timestamps are updated (upsert).

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.push_request import PushRequest
from sensecore.models.push_response import PushResponse
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
    api_instance = sensecore.ReadingsApi(api_client)
    push_request = sensecore.PushRequest() # PushRequest | 

    try:
        # Push Readings
        api_response = api_instance.push_readings_api_v1_readings_push_post(push_request)
        print("The response of ReadingsApi->push_readings_api_v1_readings_push_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReadingsApi->push_readings_api_v1_readings_push_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **push_request** | [**PushRequest**](PushRequest.md)|  | 

### Return type

[**PushResponse**](PushResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

