# sensecore.ForecastApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**forecast_api_v1_forecast_post**](ForecastApi.md#forecast_api_v1_forecast_post) | **POST** /api/v1/forecast | Forecast


# **forecast_api_v1_forecast_post**
> ForecastResponse forecast_api_v1_forecast_post(forecast_request, x_api_key=x_api_key)

Forecast

SenseCore AI — Full energy intelligence bundle.

**Input:** 336+ half-hourly meter readings (7 days minimum)

**Returns:**
- 48-period TFT forecast with 80% prediction interval
- Carbon intensity layer (Scope 2, SECR-ready)
- Anomaly detection flags
- Fuel poverty risk score (FPRS — 5 signals)
- Occupancy inference
- Cost estimate at current UK tariff

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.forecast_request import ForecastRequest
from sensecore.models.forecast_response import ForecastResponse
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
    api_instance = sensecore.ForecastApi(api_client)
    forecast_request = sensecore.ForecastRequest() # ForecastRequest | 
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Forecast
        api_response = api_instance.forecast_api_v1_forecast_post(forecast_request, x_api_key=x_api_key)
        print("The response of ForecastApi->forecast_api_v1_forecast_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ForecastApi->forecast_api_v1_forecast_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **forecast_request** | [**ForecastRequest**](ForecastRequest.md)|  | 
 **x_api_key** | **str**|  | [optional] 

### Return type

[**ForecastResponse**](ForecastResponse.md)

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

