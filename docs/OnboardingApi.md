# sensecore.OnboardingApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**complete_tour_api_v1_onboarding_complete_tour_post**](OnboardingApi.md#complete_tour_api_v1_onboarding_complete_tour_post) | **POST** /api/v1/onboarding/complete-tour | Complete Tour
[**dismiss_checklist_api_v1_onboarding_dismiss_post**](OnboardingApi.md#dismiss_checklist_api_v1_onboarding_dismiss_post) | **POST** /api/v1/onboarding/dismiss | Dismiss Checklist
[**get_status_api_v1_onboarding_status_get**](OnboardingApi.md#get_status_api_v1_onboarding_status_get) | **GET** /api/v1/onboarding/status | Get Status
[**mark_forecast_run_api_v1_onboarding_mark_forecast_run_post**](OnboardingApi.md#mark_forecast_run_api_v1_onboarding_mark_forecast_run_post) | **POST** /api/v1/onboarding/mark-forecast-run | Mark Forecast Run
[**reopen_checklist_api_v1_onboarding_reopen_post**](OnboardingApi.md#reopen_checklist_api_v1_onboarding_reopen_post) | **POST** /api/v1/onboarding/reopen | Reopen Checklist
[**set_persona_api_v1_onboarding_persona_post**](OnboardingApi.md#set_persona_api_v1_onboarding_persona_post) | **POST** /api/v1/onboarding/persona | Set Persona


# **complete_tour_api_v1_onboarding_complete_tour_post**
> SimpleOk complete_tour_api_v1_onboarding_complete_tour_post()

Complete Tour

Mark the spotlight tour as completed/skipped so it never reappears.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.simple_ok import SimpleOk
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
    api_instance = sensecore.OnboardingApi(api_client)

    try:
        # Complete Tour
        api_response = api_instance.complete_tour_api_v1_onboarding_complete_tour_post()
        print("The response of OnboardingApi->complete_tour_api_v1_onboarding_complete_tour_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingApi->complete_tour_api_v1_onboarding_complete_tour_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SimpleOk**](SimpleOk.md)

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

# **dismiss_checklist_api_v1_onboarding_dismiss_post**
> SimpleOk dismiss_checklist_api_v1_onboarding_dismiss_post()

Dismiss Checklist

Mark the floating checklist as dismissed (it can still be reopened).

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.simple_ok import SimpleOk
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
    api_instance = sensecore.OnboardingApi(api_client)

    try:
        # Dismiss Checklist
        api_response = api_instance.dismiss_checklist_api_v1_onboarding_dismiss_post()
        print("The response of OnboardingApi->dismiss_checklist_api_v1_onboarding_dismiss_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingApi->dismiss_checklist_api_v1_onboarding_dismiss_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SimpleOk**](SimpleOk.md)

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

# **get_status_api_v1_onboarding_status_get**
> OnboardingStatus get_status_api_v1_onboarding_status_get()

Get Status

Return current onboarding state for the authenticated user.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.onboarding_status import OnboardingStatus
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
    api_instance = sensecore.OnboardingApi(api_client)

    try:
        # Get Status
        api_response = api_instance.get_status_api_v1_onboarding_status_get()
        print("The response of OnboardingApi->get_status_api_v1_onboarding_status_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingApi->get_status_api_v1_onboarding_status_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**OnboardingStatus**](OnboardingStatus.md)

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

# **mark_forecast_run_api_v1_onboarding_mark_forecast_run_post**
> SimpleOk mark_forecast_run_api_v1_onboarding_mark_forecast_run_post()

Mark Forecast Run

Set the flag indicating the user clicked Run Forecast at least once.
Used as a fallback when forecast_results table is unavailable.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.simple_ok import SimpleOk
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
    api_instance = sensecore.OnboardingApi(api_client)

    try:
        # Mark Forecast Run
        api_response = api_instance.mark_forecast_run_api_v1_onboarding_mark_forecast_run_post()
        print("The response of OnboardingApi->mark_forecast_run_api_v1_onboarding_mark_forecast_run_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingApi->mark_forecast_run_api_v1_onboarding_mark_forecast_run_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SimpleOk**](SimpleOk.md)

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

# **reopen_checklist_api_v1_onboarding_reopen_post**
> SimpleOk reopen_checklist_api_v1_onboarding_reopen_post()

Reopen Checklist

Clear the dismissed flag so the checklist reappears.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.simple_ok import SimpleOk
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
    api_instance = sensecore.OnboardingApi(api_client)

    try:
        # Reopen Checklist
        api_response = api_instance.reopen_checklist_api_v1_onboarding_reopen_post()
        print("The response of OnboardingApi->reopen_checklist_api_v1_onboarding_reopen_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingApi->reopen_checklist_api_v1_onboarding_reopen_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**SimpleOk**](SimpleOk.md)

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

# **set_persona_api_v1_onboarding_persona_post**
> SimpleOk set_persona_api_v1_onboarding_persona_post(persona_request)

Set Persona

Record the user's persona and optionally seed sector-specific demo buildings.

### Example

* OAuth Authentication (OAuth2PasswordBearer):

```python
import sensecore
from sensecore.models.persona_request import PersonaRequest
from sensecore.models.simple_ok import SimpleOk
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
    api_instance = sensecore.OnboardingApi(api_client)
    persona_request = sensecore.PersonaRequest() # PersonaRequest | 

    try:
        # Set Persona
        api_response = api_instance.set_persona_api_v1_onboarding_persona_post(persona_request)
        print("The response of OnboardingApi->set_persona_api_v1_onboarding_persona_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnboardingApi->set_persona_api_v1_onboarding_persona_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **persona_request** | [**PersonaRequest**](PersonaRequest.md)|  | 

### Return type

[**SimpleOk**](SimpleOk.md)

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

