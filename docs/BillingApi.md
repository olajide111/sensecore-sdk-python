# sensecore.BillingApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_invoice_detail_api_v1_billing_invoice_invoice_id_get**](BillingApi.md#get_invoice_detail_api_v1_billing_invoice_invoice_id_get) | **GET** /api/v1/billing/invoice/{invoice_id} | Get Invoice Detail
[**get_invoice_detail_api_v1_billing_invoice_invoice_id_get_0**](BillingApi.md#get_invoice_detail_api_v1_billing_invoice_invoice_id_get_0) | **GET** /api/v1/billing/invoice/{invoice_id} | Get Invoice Detail
[**get_invoices_api_v1_billing_invoices_get**](BillingApi.md#get_invoices_api_v1_billing_invoices_get) | **GET** /api/v1/billing/invoices | Get Invoices
[**get_invoices_api_v1_billing_invoices_get_0**](BillingApi.md#get_invoices_api_v1_billing_invoices_get_0) | **GET** /api/v1/billing/invoices | Get Invoices
[**get_my_plan_api_v1_billing_my_plan_get**](BillingApi.md#get_my_plan_api_v1_billing_my_plan_get) | **GET** /api/v1/billing/my-plan | Get current org plan details and feature access
[**get_my_plan_api_v1_billing_my_plan_get_0**](BillingApi.md#get_my_plan_api_v1_billing_my_plan_get_0) | **GET** /api/v1/billing/my-plan | Get current org plan details and feature access
[**get_my_plan_api_v1_billing_my_plan_get_1**](BillingApi.md#get_my_plan_api_v1_billing_my_plan_get_1) | **GET** /api/v1/billing/my-plan | Get current org plan details and feature access
[**get_payment_settings_api_v1_billing_payment_settings_get**](BillingApi.md#get_payment_settings_api_v1_billing_payment_settings_get) | **GET** /api/v1/billing/payment-settings | Get Payment Settings
[**get_payment_settings_api_v1_billing_payment_settings_get_0**](BillingApi.md#get_payment_settings_api_v1_billing_payment_settings_get_0) | **GET** /api/v1/billing/payment-settings | Get Payment Settings
[**get_payment_settings_api_v1_billing_payment_settings_get_1**](BillingApi.md#get_payment_settings_api_v1_billing_payment_settings_get_1) | **GET** /api/v1/billing/payment-settings | Get Payment Settings
[**get_plan_api_v1_billing_plan_get**](BillingApi.md#get_plan_api_v1_billing_plan_get) | **GET** /api/v1/billing/plan | Get Plan
[**get_plan_api_v1_billing_plan_get_0**](BillingApi.md#get_plan_api_v1_billing_plan_get_0) | **GET** /api/v1/billing/plan | Get Plan
[**request_invoice_api_v1_billing_invoices_request_post**](BillingApi.md#request_invoice_api_v1_billing_invoices_request_post) | **POST** /api/v1/billing/invoices/request | Request Invoice
[**request_invoice_api_v1_billing_invoices_request_post_0**](BillingApi.md#request_invoice_api_v1_billing_invoices_request_post_0) | **POST** /api/v1/billing/invoices/request | Request Invoice
[**update_plan_api_v1_billing_plan_post**](BillingApi.md#update_plan_api_v1_billing_plan_post) | **POST** /api/v1/billing/plan | Update Plan
[**update_plan_api_v1_billing_plan_post_0**](BillingApi.md#update_plan_api_v1_billing_plan_post_0) | **POST** /api/v1/billing/plan | Update Plan


# **get_invoice_detail_api_v1_billing_invoice_invoice_id_get**
> object get_invoice_detail_api_v1_billing_invoice_invoice_id_get(invoice_id)

Get Invoice Detail

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
    api_instance = sensecore.BillingApi(api_client)
    invoice_id = 'invoice_id_example' # str | Invoice ID or number

    try:
        # Get Invoice Detail
        api_response = api_instance.get_invoice_detail_api_v1_billing_invoice_invoice_id_get(invoice_id)
        print("The response of BillingApi->get_invoice_detail_api_v1_billing_invoice_invoice_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_invoice_detail_api_v1_billing_invoice_invoice_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**| Invoice ID or number | 

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

# **get_invoice_detail_api_v1_billing_invoice_invoice_id_get_0**
> object get_invoice_detail_api_v1_billing_invoice_invoice_id_get_0(invoice_id)

Get Invoice Detail

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
    api_instance = sensecore.BillingApi(api_client)
    invoice_id = 'invoice_id_example' # str | Invoice ID or number

    try:
        # Get Invoice Detail
        api_response = api_instance.get_invoice_detail_api_v1_billing_invoice_invoice_id_get_0(invoice_id)
        print("The response of BillingApi->get_invoice_detail_api_v1_billing_invoice_invoice_id_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_invoice_detail_api_v1_billing_invoice_invoice_id_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**| Invoice ID or number | 

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

# **get_invoices_api_v1_billing_invoices_get**
> List[object] get_invoices_api_v1_billing_invoices_get()

Get Invoices

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
    api_instance = sensecore.BillingApi(api_client)

    try:
        # Get Invoices
        api_response = api_instance.get_invoices_api_v1_billing_invoices_get()
        print("The response of BillingApi->get_invoices_api_v1_billing_invoices_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_invoices_api_v1_billing_invoices_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**List[object]**

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

# **get_invoices_api_v1_billing_invoices_get_0**
> List[object] get_invoices_api_v1_billing_invoices_get_0()

Get Invoices

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
    api_instance = sensecore.BillingApi(api_client)

    try:
        # Get Invoices
        api_response = api_instance.get_invoices_api_v1_billing_invoices_get_0()
        print("The response of BillingApi->get_invoices_api_v1_billing_invoices_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_invoices_api_v1_billing_invoices_get_0: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

**List[object]**

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

# **get_my_plan_api_v1_billing_my_plan_get**
> object get_my_plan_api_v1_billing_my_plan_get()

Get current org plan details and feature access

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
    api_instance = sensecore.BillingApi(api_client)

    try:
        # Get current org plan details and feature access
        api_response = api_instance.get_my_plan_api_v1_billing_my_plan_get()
        print("The response of BillingApi->get_my_plan_api_v1_billing_my_plan_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_my_plan_api_v1_billing_my_plan_get: %s\n" % e)
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

# **get_my_plan_api_v1_billing_my_plan_get_0**
> object get_my_plan_api_v1_billing_my_plan_get_0()

Get current org plan details and feature access

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
    api_instance = sensecore.BillingApi(api_client)

    try:
        # Get current org plan details and feature access
        api_response = api_instance.get_my_plan_api_v1_billing_my_plan_get_0()
        print("The response of BillingApi->get_my_plan_api_v1_billing_my_plan_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_my_plan_api_v1_billing_my_plan_get_0: %s\n" % e)
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

# **get_my_plan_api_v1_billing_my_plan_get_1**
> object get_my_plan_api_v1_billing_my_plan_get_1()

Get current org plan details and feature access

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
    api_instance = sensecore.BillingApi(api_client)

    try:
        # Get current org plan details and feature access
        api_response = api_instance.get_my_plan_api_v1_billing_my_plan_get_1()
        print("The response of BillingApi->get_my_plan_api_v1_billing_my_plan_get_1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_my_plan_api_v1_billing_my_plan_get_1: %s\n" % e)
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

# **get_payment_settings_api_v1_billing_payment_settings_get**
> object get_payment_settings_api_v1_billing_payment_settings_get()

Get Payment Settings

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
    api_instance = sensecore.BillingApi(api_client)

    try:
        # Get Payment Settings
        api_response = api_instance.get_payment_settings_api_v1_billing_payment_settings_get()
        print("The response of BillingApi->get_payment_settings_api_v1_billing_payment_settings_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_payment_settings_api_v1_billing_payment_settings_get: %s\n" % e)
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

# **get_payment_settings_api_v1_billing_payment_settings_get_0**
> object get_payment_settings_api_v1_billing_payment_settings_get_0()

Get Payment Settings

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
    api_instance = sensecore.BillingApi(api_client)

    try:
        # Get Payment Settings
        api_response = api_instance.get_payment_settings_api_v1_billing_payment_settings_get_0()
        print("The response of BillingApi->get_payment_settings_api_v1_billing_payment_settings_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_payment_settings_api_v1_billing_payment_settings_get_0: %s\n" % e)
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

# **get_payment_settings_api_v1_billing_payment_settings_get_1**
> object get_payment_settings_api_v1_billing_payment_settings_get_1()

Get Payment Settings

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
    api_instance = sensecore.BillingApi(api_client)

    try:
        # Get Payment Settings
        api_response = api_instance.get_payment_settings_api_v1_billing_payment_settings_get_1()
        print("The response of BillingApi->get_payment_settings_api_v1_billing_payment_settings_get_1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_payment_settings_api_v1_billing_payment_settings_get_1: %s\n" % e)
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

# **get_plan_api_v1_billing_plan_get**
> object get_plan_api_v1_billing_plan_get()

Get Plan

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
    api_instance = sensecore.BillingApi(api_client)

    try:
        # Get Plan
        api_response = api_instance.get_plan_api_v1_billing_plan_get()
        print("The response of BillingApi->get_plan_api_v1_billing_plan_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_plan_api_v1_billing_plan_get: %s\n" % e)
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

# **get_plan_api_v1_billing_plan_get_0**
> object get_plan_api_v1_billing_plan_get_0()

Get Plan

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
    api_instance = sensecore.BillingApi(api_client)

    try:
        # Get Plan
        api_response = api_instance.get_plan_api_v1_billing_plan_get_0()
        print("The response of BillingApi->get_plan_api_v1_billing_plan_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->get_plan_api_v1_billing_plan_get_0: %s\n" % e)
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

# **request_invoice_api_v1_billing_invoices_request_post**
> object request_invoice_api_v1_billing_invoices_request_post(body)

Request Invoice

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
    api_instance = sensecore.BillingApi(api_client)
    body = None # object | 

    try:
        # Request Invoice
        api_response = api_instance.request_invoice_api_v1_billing_invoices_request_post(body)
        print("The response of BillingApi->request_invoice_api_v1_billing_invoices_request_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->request_invoice_api_v1_billing_invoices_request_post: %s\n" % e)
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

# **request_invoice_api_v1_billing_invoices_request_post_0**
> object request_invoice_api_v1_billing_invoices_request_post_0(body)

Request Invoice

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
    api_instance = sensecore.BillingApi(api_client)
    body = None # object | 

    try:
        # Request Invoice
        api_response = api_instance.request_invoice_api_v1_billing_invoices_request_post_0(body)
        print("The response of BillingApi->request_invoice_api_v1_billing_invoices_request_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->request_invoice_api_v1_billing_invoices_request_post_0: %s\n" % e)
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

# **update_plan_api_v1_billing_plan_post**
> object update_plan_api_v1_billing_plan_post(body)

Update Plan

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
    api_instance = sensecore.BillingApi(api_client)
    body = None # object | 

    try:
        # Update Plan
        api_response = api_instance.update_plan_api_v1_billing_plan_post(body)
        print("The response of BillingApi->update_plan_api_v1_billing_plan_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->update_plan_api_v1_billing_plan_post: %s\n" % e)
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

# **update_plan_api_v1_billing_plan_post_0**
> object update_plan_api_v1_billing_plan_post_0(body)

Update Plan

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
    api_instance = sensecore.BillingApi(api_client)
    body = None # object | 

    try:
        # Update Plan
        api_response = api_instance.update_plan_api_v1_billing_plan_post_0(body)
        print("The response of BillingApi->update_plan_api_v1_billing_plan_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingApi->update_plan_api_v1_billing_plan_post_0: %s\n" % e)
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

