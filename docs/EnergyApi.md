# sensecore.EnergyApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**energy_forecast_api_v1_energy_forecast_post**](EnergyApi.md#energy_forecast_api_v1_energy_forecast_post) | **POST** /api/v1/energy/forecast | Energy Forecast
[**energy_forecast_api_v1_energy_forecast_post_0**](EnergyApi.md#energy_forecast_api_v1_energy_forecast_post_0) | **POST** /api/v1/energy/forecast | Energy Forecast
[**get_energy_types_api_v1_energy_types_get**](EnergyApi.md#get_energy_types_api_v1_energy_types_get) | **GET** /api/v1/energy/types | Get Energy Types
[**get_energy_types_api_v1_energy_types_get_0**](EnergyApi.md#get_energy_types_api_v1_energy_types_get_0) | **GET** /api/v1/energy/types | Get Energy Types
[**get_weather_data_api_v1_energy_weather_get**](EnergyApi.md#get_weather_data_api_v1_energy_weather_get) | **GET** /api/v1/energy/weather | Get Weather Data
[**get_weather_data_api_v1_energy_weather_get_0**](EnergyApi.md#get_weather_data_api_v1_energy_weather_get_0) | **GET** /api/v1/energy/weather | Get Weather Data
[**toggle_energy_type_api_v1_energy_types_toggle_post**](EnergyApi.md#toggle_energy_type_api_v1_energy_types_toggle_post) | **POST** /api/v1/energy/types/toggle | Toggle Energy Type
[**toggle_energy_type_api_v1_energy_types_toggle_post_0**](EnergyApi.md#toggle_energy_type_api_v1_energy_types_toggle_post_0) | **POST** /api/v1/energy/types/toggle | Toggle Energy Type


# **energy_forecast_api_v1_energy_forecast_post**
> object energy_forecast_api_v1_energy_forecast_post(energy_forecast_request, type=type)

Energy Forecast

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.energy_forecast_request import EnergyForecastRequest
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
    api_instance = sensecore.EnergyApi(api_client)
    energy_forecast_request = sensecore.EnergyForecastRequest() # EnergyForecastRequest | 
    type = 'electricity' # str |  (optional) (default to 'electricity')

    try:
        # Energy Forecast
        api_response = api_instance.energy_forecast_api_v1_energy_forecast_post(energy_forecast_request, type=type)
        print("The response of EnergyApi->energy_forecast_api_v1_energy_forecast_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnergyApi->energy_forecast_api_v1_energy_forecast_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **energy_forecast_request** | [**EnergyForecastRequest**](EnergyForecastRequest.md)|  | 
 **type** | **str**|  | [optional] [default to &#39;electricity&#39;]

### Return type

**object**

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

# **energy_forecast_api_v1_energy_forecast_post_0**
> object energy_forecast_api_v1_energy_forecast_post_0(energy_forecast_request, type=type)

Energy Forecast

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.energy_forecast_request import EnergyForecastRequest
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
    api_instance = sensecore.EnergyApi(api_client)
    energy_forecast_request = sensecore.EnergyForecastRequest() # EnergyForecastRequest | 
    type = 'electricity' # str |  (optional) (default to 'electricity')

    try:
        # Energy Forecast
        api_response = api_instance.energy_forecast_api_v1_energy_forecast_post_0(energy_forecast_request, type=type)
        print("The response of EnergyApi->energy_forecast_api_v1_energy_forecast_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnergyApi->energy_forecast_api_v1_energy_forecast_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **energy_forecast_request** | [**EnergyForecastRequest**](EnergyForecastRequest.md)|  | 
 **type** | **str**|  | [optional] [default to &#39;electricity&#39;]

### Return type

**object**

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

# **get_energy_types_api_v1_energy_types_get**
> object get_energy_types_api_v1_energy_types_get()

Get Energy Types

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
    api_instance = sensecore.EnergyApi(api_client)

    try:
        # Get Energy Types
        api_response = api_instance.get_energy_types_api_v1_energy_types_get()
        print("The response of EnergyApi->get_energy_types_api_v1_energy_types_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnergyApi->get_energy_types_api_v1_energy_types_get: %s\n" % e)
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

# **get_energy_types_api_v1_energy_types_get_0**
> object get_energy_types_api_v1_energy_types_get_0()

Get Energy Types

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
    api_instance = sensecore.EnergyApi(api_client)

    try:
        # Get Energy Types
        api_response = api_instance.get_energy_types_api_v1_energy_types_get_0()
        print("The response of EnergyApi->get_energy_types_api_v1_energy_types_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnergyApi->get_energy_types_api_v1_energy_types_get_0: %s\n" % e)
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

# **get_weather_data_api_v1_energy_weather_get**
> object get_weather_data_api_v1_energy_weather_get(lat=lat, lon=lon, days=days)

Get Weather Data

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
    api_instance = sensecore.EnergyApi(api_client)
    lat = 51.5074 # float |  (optional) (default to 51.5074)
    lon = -0.1278 # float |  (optional) (default to -0.1278)
    days = 7 # int |  (optional) (default to 7)

    try:
        # Get Weather Data
        api_response = api_instance.get_weather_data_api_v1_energy_weather_get(lat=lat, lon=lon, days=days)
        print("The response of EnergyApi->get_weather_data_api_v1_energy_weather_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnergyApi->get_weather_data_api_v1_energy_weather_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lat** | **float**|  | [optional] [default to 51.5074]
 **lon** | **float**|  | [optional] [default to -0.1278]
 **days** | **int**|  | [optional] [default to 7]

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

# **get_weather_data_api_v1_energy_weather_get_0**
> object get_weather_data_api_v1_energy_weather_get_0(lat=lat, lon=lon, days=days)

Get Weather Data

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
    api_instance = sensecore.EnergyApi(api_client)
    lat = 51.5074 # float |  (optional) (default to 51.5074)
    lon = -0.1278 # float |  (optional) (default to -0.1278)
    days = 7 # int |  (optional) (default to 7)

    try:
        # Get Weather Data
        api_response = api_instance.get_weather_data_api_v1_energy_weather_get_0(lat=lat, lon=lon, days=days)
        print("The response of EnergyApi->get_weather_data_api_v1_energy_weather_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnergyApi->get_weather_data_api_v1_energy_weather_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lat** | **float**|  | [optional] [default to 51.5074]
 **lon** | **float**|  | [optional] [default to -0.1278]
 **days** | **int**|  | [optional] [default to 7]

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

# **toggle_energy_type_api_v1_energy_types_toggle_post**
> object toggle_energy_type_api_v1_energy_types_toggle_post(body)

Toggle Energy Type

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
    api_instance = sensecore.EnergyApi(api_client)
    body = None # object | 

    try:
        # Toggle Energy Type
        api_response = api_instance.toggle_energy_type_api_v1_energy_types_toggle_post(body)
        print("The response of EnergyApi->toggle_energy_type_api_v1_energy_types_toggle_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnergyApi->toggle_energy_type_api_v1_energy_types_toggle_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | 

### Return type

**object**

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

# **toggle_energy_type_api_v1_energy_types_toggle_post_0**
> object toggle_energy_type_api_v1_energy_types_toggle_post_0(body)

Toggle Energy Type

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
    api_instance = sensecore.EnergyApi(api_client)
    body = None # object | 

    try:
        # Toggle Energy Type
        api_response = api_instance.toggle_energy_type_api_v1_energy_types_toggle_post_0(body)
        print("The response of EnergyApi->toggle_energy_type_api_v1_energy_types_toggle_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling EnergyApi->toggle_energy_type_api_v1_energy_types_toggle_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | 

### Return type

**object**

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

