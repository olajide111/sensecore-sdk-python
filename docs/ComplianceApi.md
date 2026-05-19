# sensecore.ComplianceApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generate_eric_api_v1_compliance_eric_post**](ComplianceApi.md#generate_eric_api_v1_compliance_eric_post) | **POST** /api/v1/compliance/eric | Generate Eric
[**generate_eric_api_v1_compliance_eric_post_0**](ComplianceApi.md#generate_eric_api_v1_compliance_eric_post_0) | **POST** /api/v1/compliance/eric | Generate Eric
[**generate_esos_api_v1_compliance_esos_post**](ComplianceApi.md#generate_esos_api_v1_compliance_esos_post) | **POST** /api/v1/compliance/esos | Generate Esos
[**generate_esos_api_v1_compliance_esos_post_0**](ComplianceApi.md#generate_esos_api_v1_compliance_esos_post_0) | **POST** /api/v1/compliance/esos | Generate Esos
[**generate_secr_api_v1_compliance_secr_post**](ComplianceApi.md#generate_secr_api_v1_compliance_secr_post) | **POST** /api/v1/compliance/secr | Generate Secr
[**generate_secr_api_v1_compliance_secr_post_0**](ComplianceApi.md#generate_secr_api_v1_compliance_secr_post_0) | **POST** /api/v1/compliance/secr | Generate Secr
[**generate_shdf_api_v1_compliance_shdf_post**](ComplianceApi.md#generate_shdf_api_v1_compliance_shdf_post) | **POST** /api/v1/compliance/shdf | Generate Shdf
[**generate_shdf_api_v1_compliance_shdf_post_0**](ComplianceApi.md#generate_shdf_api_v1_compliance_shdf_post_0) | **POST** /api/v1/compliance/shdf | Generate Shdf
[**get_epc_tracking_api_v1_compliance_epc_get**](ComplianceApi.md#get_epc_tracking_api_v1_compliance_epc_get) | **GET** /api/v1/compliance/epc | Get Epc Tracking
[**get_epc_tracking_api_v1_compliance_epc_get_0**](ComplianceApi.md#get_epc_tracking_api_v1_compliance_epc_get_0) | **GET** /api/v1/compliance/epc | Get Epc Tracking


# **generate_eric_api_v1_compliance_eric_post**
> ERICResponse generate_eric_api_v1_compliance_eric_post(compliance_request, x_api_key=x_api_key)

Generate Eric

Generate NHS Estates Returns Information Collection (ERIC) energy data.
ERIC requires: electricity, gas, oil, coal, steam, hot water consumption
in kWh and GJ, plus CO2 emissions, floor area, and energy cost.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.compliance_request import ComplianceRequest
from sensecore.models.eric_response import ERICResponse
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
    api_instance = sensecore.ComplianceApi(api_client)
    compliance_request = sensecore.ComplianceRequest() # ComplianceRequest | 
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Generate Eric
        api_response = api_instance.generate_eric_api_v1_compliance_eric_post(compliance_request, x_api_key=x_api_key)
        print("The response of ComplianceApi->generate_eric_api_v1_compliance_eric_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->generate_eric_api_v1_compliance_eric_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **compliance_request** | [**ComplianceRequest**](ComplianceRequest.md)|  | 
 **x_api_key** | **str**|  | [optional] 

### Return type

[**ERICResponse**](ERICResponse.md)

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

# **generate_eric_api_v1_compliance_eric_post_0**
> ERICResponse generate_eric_api_v1_compliance_eric_post_0(compliance_request, x_api_key=x_api_key)

Generate Eric

Generate NHS Estates Returns Information Collection (ERIC) energy data.
ERIC requires: electricity, gas, oil, coal, steam, hot water consumption
in kWh and GJ, plus CO2 emissions, floor area, and energy cost.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.compliance_request import ComplianceRequest
from sensecore.models.eric_response import ERICResponse
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
    api_instance = sensecore.ComplianceApi(api_client)
    compliance_request = sensecore.ComplianceRequest() # ComplianceRequest | 
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Generate Eric
        api_response = api_instance.generate_eric_api_v1_compliance_eric_post_0(compliance_request, x_api_key=x_api_key)
        print("The response of ComplianceApi->generate_eric_api_v1_compliance_eric_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->generate_eric_api_v1_compliance_eric_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **compliance_request** | [**ComplianceRequest**](ComplianceRequest.md)|  | 
 **x_api_key** | **str**|  | [optional] 

### Return type

[**ERICResponse**](ERICResponse.md)

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

# **generate_esos_api_v1_compliance_esos_post**
> ESOSResponse generate_esos_api_v1_compliance_esos_post(compliance_request, x_api_key=x_api_key)

Generate Esos

Generate ESOS Phase 4 evidence pack.
ESOS requires energy audits covering at least 90% of total energy,
identification of energy savings opportunities, and lead assessor sign-off.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.compliance_request import ComplianceRequest
from sensecore.models.esos_response import ESOSResponse
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
    api_instance = sensecore.ComplianceApi(api_client)
    compliance_request = sensecore.ComplianceRequest() # ComplianceRequest | 
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Generate Esos
        api_response = api_instance.generate_esos_api_v1_compliance_esos_post(compliance_request, x_api_key=x_api_key)
        print("The response of ComplianceApi->generate_esos_api_v1_compliance_esos_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->generate_esos_api_v1_compliance_esos_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **compliance_request** | [**ComplianceRequest**](ComplianceRequest.md)|  | 
 **x_api_key** | **str**|  | [optional] 

### Return type

[**ESOSResponse**](ESOSResponse.md)

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

# **generate_esos_api_v1_compliance_esos_post_0**
> ESOSResponse generate_esos_api_v1_compliance_esos_post_0(compliance_request, x_api_key=x_api_key)

Generate Esos

Generate ESOS Phase 4 evidence pack.
ESOS requires energy audits covering at least 90% of total energy,
identification of energy savings opportunities, and lead assessor sign-off.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.compliance_request import ComplianceRequest
from sensecore.models.esos_response import ESOSResponse
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
    api_instance = sensecore.ComplianceApi(api_client)
    compliance_request = sensecore.ComplianceRequest() # ComplianceRequest | 
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Generate Esos
        api_response = api_instance.generate_esos_api_v1_compliance_esos_post_0(compliance_request, x_api_key=x_api_key)
        print("The response of ComplianceApi->generate_esos_api_v1_compliance_esos_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->generate_esos_api_v1_compliance_esos_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **compliance_request** | [**ComplianceRequest**](ComplianceRequest.md)|  | 
 **x_api_key** | **str**|  | [optional] 

### Return type

[**ESOSResponse**](ESOSResponse.md)

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

# **generate_secr_api_v1_compliance_secr_post**
> SECRResponse generate_secr_api_v1_compliance_secr_post(compliance_request, x_api_key=x_api_key)

Generate Secr

Generate Streamlined Energy and Carbon Report.
SECR requires: Scope 1+2 emissions, at least one intensity ratio,
prior year comparatives, and energy efficiency narrative.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.compliance_request import ComplianceRequest
from sensecore.models.secr_response import SECRResponse
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
    api_instance = sensecore.ComplianceApi(api_client)
    compliance_request = sensecore.ComplianceRequest() # ComplianceRequest | 
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Generate Secr
        api_response = api_instance.generate_secr_api_v1_compliance_secr_post(compliance_request, x_api_key=x_api_key)
        print("The response of ComplianceApi->generate_secr_api_v1_compliance_secr_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->generate_secr_api_v1_compliance_secr_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **compliance_request** | [**ComplianceRequest**](ComplianceRequest.md)|  | 
 **x_api_key** | **str**|  | [optional] 

### Return type

[**SECRResponse**](SECRResponse.md)

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

# **generate_secr_api_v1_compliance_secr_post_0**
> SECRResponse generate_secr_api_v1_compliance_secr_post_0(compliance_request, x_api_key=x_api_key)

Generate Secr

Generate Streamlined Energy and Carbon Report.
SECR requires: Scope 1+2 emissions, at least one intensity ratio,
prior year comparatives, and energy efficiency narrative.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.compliance_request import ComplianceRequest
from sensecore.models.secr_response import SECRResponse
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
    api_instance = sensecore.ComplianceApi(api_client)
    compliance_request = sensecore.ComplianceRequest() # ComplianceRequest | 
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Generate Secr
        api_response = api_instance.generate_secr_api_v1_compliance_secr_post_0(compliance_request, x_api_key=x_api_key)
        print("The response of ComplianceApi->generate_secr_api_v1_compliance_secr_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->generate_secr_api_v1_compliance_secr_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **compliance_request** | [**ComplianceRequest**](ComplianceRequest.md)|  | 
 **x_api_key** | **str**|  | [optional] 

### Return type

[**SECRResponse**](SECRResponse.md)

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

# **generate_shdf_api_v1_compliance_shdf_post**
> SHDFResponse generate_shdf_api_v1_compliance_shdf_post(compliance_request, x_api_key=x_api_key)

Generate Shdf

Generate Social Housing Decarbonisation Fund (SHDF) readiness assessment.
Uses FPRS scores to identify properties eligible for Wave 2 funding.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.compliance_request import ComplianceRequest
from sensecore.models.shdf_response import SHDFResponse
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
    api_instance = sensecore.ComplianceApi(api_client)
    compliance_request = sensecore.ComplianceRequest() # ComplianceRequest | 
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Generate Shdf
        api_response = api_instance.generate_shdf_api_v1_compliance_shdf_post(compliance_request, x_api_key=x_api_key)
        print("The response of ComplianceApi->generate_shdf_api_v1_compliance_shdf_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->generate_shdf_api_v1_compliance_shdf_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **compliance_request** | [**ComplianceRequest**](ComplianceRequest.md)|  | 
 **x_api_key** | **str**|  | [optional] 

### Return type

[**SHDFResponse**](SHDFResponse.md)

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

# **generate_shdf_api_v1_compliance_shdf_post_0**
> SHDFResponse generate_shdf_api_v1_compliance_shdf_post_0(compliance_request, x_api_key=x_api_key)

Generate Shdf

Generate Social Housing Decarbonisation Fund (SHDF) readiness assessment.
Uses FPRS scores to identify properties eligible for Wave 2 funding.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.compliance_request import ComplianceRequest
from sensecore.models.shdf_response import SHDFResponse
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
    api_instance = sensecore.ComplianceApi(api_client)
    compliance_request = sensecore.ComplianceRequest() # ComplianceRequest | 
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Generate Shdf
        api_response = api_instance.generate_shdf_api_v1_compliance_shdf_post_0(compliance_request, x_api_key=x_api_key)
        print("The response of ComplianceApi->generate_shdf_api_v1_compliance_shdf_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->generate_shdf_api_v1_compliance_shdf_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **compliance_request** | [**ComplianceRequest**](ComplianceRequest.md)|  | 
 **x_api_key** | **str**|  | [optional] 

### Return type

[**SHDFResponse**](SHDFResponse.md)

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

# **get_epc_tracking_api_v1_compliance_epc_get**
> object get_epc_tracking_api_v1_compliance_epc_get(x_api_key=x_api_key)

Get Epc Tracking

Get EPC band tracking for all buildings in the organisation.
Returns current bands, target bands, and recommendations.

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
    api_instance = sensecore.ComplianceApi(api_client)
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Get Epc Tracking
        api_response = api_instance.get_epc_tracking_api_v1_compliance_epc_get(x_api_key=x_api_key)
        print("The response of ComplianceApi->get_epc_tracking_api_v1_compliance_epc_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->get_epc_tracking_api_v1_compliance_epc_get: %s\n" % e)
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

# **get_epc_tracking_api_v1_compliance_epc_get_0**
> object get_epc_tracking_api_v1_compliance_epc_get_0(x_api_key=x_api_key)

Get Epc Tracking

Get EPC band tracking for all buildings in the organisation.
Returns current bands, target bands, and recommendations.

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
    api_instance = sensecore.ComplianceApi(api_client)
    x_api_key = 'x_api_key_example' # str |  (optional)

    try:
        # Get Epc Tracking
        api_response = api_instance.get_epc_tracking_api_v1_compliance_epc_get_0(x_api_key=x_api_key)
        print("The response of ComplianceApi->get_epc_tracking_api_v1_compliance_epc_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ComplianceApi->get_epc_tracking_api_v1_compliance_epc_get_0: %s\n" % e)
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

