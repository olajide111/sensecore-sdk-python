# sensecore.CarbonApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**carbon_report_api_v1_carbon_post**](CarbonApi.md#carbon_report_api_v1_carbon_post) | **POST** /api/v1/carbon | Carbon Report


# **carbon_report_api_v1_carbon_post**
> CarbonResponse carbon_report_api_v1_carbon_post(carbon_request)

Carbon Report

Generate a Scope 2 carbon report from meter readings.
SECR and EU EED compliant. Uses BEIS carbon intensity factors.
Suitable for NHS sustainability returns, PSDS reporting, and SECR filings.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.carbon_request import CarbonRequest
from sensecore.models.carbon_response import CarbonResponse
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
    api_instance = sensecore.CarbonApi(api_client)
    carbon_request = sensecore.CarbonRequest() # CarbonRequest | 

    try:
        # Carbon Report
        api_response = api_instance.carbon_report_api_v1_carbon_post(carbon_request)
        print("The response of CarbonApi->carbon_report_api_v1_carbon_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CarbonApi->carbon_report_api_v1_carbon_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **carbon_request** | [**CarbonRequest**](CarbonRequest.md)|  | 

### Return type

[**CarbonResponse**](CarbonResponse.md)

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

