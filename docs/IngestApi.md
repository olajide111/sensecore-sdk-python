# sensecore.IngestApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ingest_api_v1_ingest_post**](IngestApi.md#ingest_api_v1_ingest_post) | **POST** /api/v1/ingest | Ingest


# **ingest_api_v1_ingest_post**
> IngestResponse ingest_api_v1_ingest_post(meter_id, file, x_api_key=x_api_key)

Ingest

Upload a CSV of half-hourly meter readings.
Accepts exports from Octopus Energy, British Gas, EON, and most UK suppliers.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.ingest_response import IngestResponse
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
    api_instance = sensecore.IngestApi(api_client)
    meter_id = 'meter_id_example' # str | 
    file = None # bytes | 
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Ingest
        api_response = api_instance.ingest_api_v1_ingest_post(meter_id, file, x_api_key=x_api_key)
        print("The response of IngestApi->ingest_api_v1_ingest_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling IngestApi->ingest_api_v1_ingest_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **meter_id** | **str**|  | 
 **file** | **bytes**|  | 
 **x_api_key** | **str**|  | [optional] 

### Return type

[**IngestResponse**](IngestResponse.md)

### Authorization

[OAuth2PasswordBearer](../README.md#OAuth2PasswordBearer)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

