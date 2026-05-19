# sensecore.OptimiseApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**optimise_api_v1_optimise_post**](OptimiseApi.md#optimise_api_v1_optimise_post) | **POST** /api/v1/optimise | Optimise


# **optimise_api_v1_optimise_post**
> OptimiseResponse optimise_api_v1_optimise_post(optimise_request, x_api_key=x_api_key)

Optimise

Compare UK energy tariffs using actual consumption data.
Returns best tariff and estimated annual saving in GBP.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.optimise_request import OptimiseRequest
from sensecore.models.optimise_response import OptimiseResponse
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
    api_instance = sensecore.OptimiseApi(api_client)
    optimise_request = sensecore.OptimiseRequest() # OptimiseRequest | 
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Optimise
        api_response = api_instance.optimise_api_v1_optimise_post(optimise_request, x_api_key=x_api_key)
        print("The response of OptimiseApi->optimise_api_v1_optimise_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OptimiseApi->optimise_api_v1_optimise_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **optimise_request** | [**OptimiseRequest**](OptimiseRequest.md)|  | 
 **x_api_key** | **str**|  | [optional] 

### Return type

[**OptimiseResponse**](OptimiseResponse.md)

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

