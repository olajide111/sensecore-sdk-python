# sensecore.AIGovernanceApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ai_transparency_api_v1_ai_transparency_get**](AIGovernanceApi.md#ai_transparency_api_v1_ai_transparency_get) | **GET** /api/v1/ai/transparency | Ai Transparency
[**ai_transparency_api_v1_ai_transparency_get_0**](AIGovernanceApi.md#ai_transparency_api_v1_ai_transparency_get_0) | **GET** /api/v1/ai/transparency | Ai Transparency
[**bias_assessment_api_v1_ai_bias_assessment_get**](AIGovernanceApi.md#bias_assessment_api_v1_ai_bias_assessment_get) | **GET** /api/v1/ai/bias-assessment | Bias Assessment
[**bias_assessment_api_v1_ai_bias_assessment_get_0**](AIGovernanceApi.md#bias_assessment_api_v1_ai_bias_assessment_get_0) | **GET** /api/v1/ai/bias-assessment | Bias Assessment
[**get_model_detail_api_v1_ai_models_model_id_get**](AIGovernanceApi.md#get_model_detail_api_v1_ai_models_model_id_get) | **GET** /api/v1/ai/models/{model_id} | Get Model Detail
[**get_model_detail_api_v1_ai_models_model_id_get_0**](AIGovernanceApi.md#get_model_detail_api_v1_ai_models_model_id_get_0) | **GET** /api/v1/ai/models/{model_id} | Get Model Detail
[**list_models_api_v1_ai_models_get**](AIGovernanceApi.md#list_models_api_v1_ai_models_get) | **GET** /api/v1/ai/models | List Models
[**list_models_api_v1_ai_models_get_0**](AIGovernanceApi.md#list_models_api_v1_ai_models_get_0) | **GET** /api/v1/ai/models | List Models


# **ai_transparency_api_v1_ai_transparency_get**
> object ai_transparency_api_v1_ai_transparency_get()

Ai Transparency

EU AI Act Article 13 transparency information.

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
    api_instance = sensecore.AIGovernanceApi(api_client)

    try:
        # Ai Transparency
        api_response = api_instance.ai_transparency_api_v1_ai_transparency_get()
        print("The response of AIGovernanceApi->ai_transparency_api_v1_ai_transparency_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AIGovernanceApi->ai_transparency_api_v1_ai_transparency_get: %s\n" % e)
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

# **ai_transparency_api_v1_ai_transparency_get_0**
> object ai_transparency_api_v1_ai_transparency_get_0()

Ai Transparency

EU AI Act Article 13 transparency information.

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
    api_instance = sensecore.AIGovernanceApi(api_client)

    try:
        # Ai Transparency
        api_response = api_instance.ai_transparency_api_v1_ai_transparency_get_0()
        print("The response of AIGovernanceApi->ai_transparency_api_v1_ai_transparency_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AIGovernanceApi->ai_transparency_api_v1_ai_transparency_get_0: %s\n" % e)
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

# **bias_assessment_api_v1_ai_bias_assessment_get**
> object bias_assessment_api_v1_ai_bias_assessment_get()

Bias Assessment

FPRS bias assessment — protected characteristics analysis.

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
    api_instance = sensecore.AIGovernanceApi(api_client)

    try:
        # Bias Assessment
        api_response = api_instance.bias_assessment_api_v1_ai_bias_assessment_get()
        print("The response of AIGovernanceApi->bias_assessment_api_v1_ai_bias_assessment_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AIGovernanceApi->bias_assessment_api_v1_ai_bias_assessment_get: %s\n" % e)
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

# **bias_assessment_api_v1_ai_bias_assessment_get_0**
> object bias_assessment_api_v1_ai_bias_assessment_get_0()

Bias Assessment

FPRS bias assessment — protected characteristics analysis.

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
    api_instance = sensecore.AIGovernanceApi(api_client)

    try:
        # Bias Assessment
        api_response = api_instance.bias_assessment_api_v1_ai_bias_assessment_get_0()
        print("The response of AIGovernanceApi->bias_assessment_api_v1_ai_bias_assessment_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AIGovernanceApi->bias_assessment_api_v1_ai_bias_assessment_get_0: %s\n" % e)
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

# **get_model_detail_api_v1_ai_models_model_id_get**
> object get_model_detail_api_v1_ai_models_model_id_get(model_id)

Get Model Detail

Get detailed information about a specific model.

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
    api_instance = sensecore.AIGovernanceApi(api_client)
    model_id = 'model_id_example' # str | 

    try:
        # Get Model Detail
        api_response = api_instance.get_model_detail_api_v1_ai_models_model_id_get(model_id)
        print("The response of AIGovernanceApi->get_model_detail_api_v1_ai_models_model_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AIGovernanceApi->get_model_detail_api_v1_ai_models_model_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model_id** | **str**|  | 

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

# **get_model_detail_api_v1_ai_models_model_id_get_0**
> object get_model_detail_api_v1_ai_models_model_id_get_0(model_id)

Get Model Detail

Get detailed information about a specific model.

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
    api_instance = sensecore.AIGovernanceApi(api_client)
    model_id = 'model_id_example' # str | 

    try:
        # Get Model Detail
        api_response = api_instance.get_model_detail_api_v1_ai_models_model_id_get_0(model_id)
        print("The response of AIGovernanceApi->get_model_detail_api_v1_ai_models_model_id_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AIGovernanceApi->get_model_detail_api_v1_ai_models_model_id_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **model_id** | **str**|  | 

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

# **list_models_api_v1_ai_models_get**
> object list_models_api_v1_ai_models_get()

List Models

List all deployed AI models with metadata.

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
    api_instance = sensecore.AIGovernanceApi(api_client)

    try:
        # List Models
        api_response = api_instance.list_models_api_v1_ai_models_get()
        print("The response of AIGovernanceApi->list_models_api_v1_ai_models_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AIGovernanceApi->list_models_api_v1_ai_models_get: %s\n" % e)
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

# **list_models_api_v1_ai_models_get_0**
> object list_models_api_v1_ai_models_get_0()

List Models

List all deployed AI models with metadata.

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
    api_instance = sensecore.AIGovernanceApi(api_client)

    try:
        # List Models
        api_response = api_instance.list_models_api_v1_ai_models_get_0()
        print("The response of AIGovernanceApi->list_models_api_v1_ai_models_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AIGovernanceApi->list_models_api_v1_ai_models_get_0: %s\n" % e)
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

