# sensecore.BillingEmailApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**email_all_invoices_api_v1_billing_invoices_email_all_post**](BillingEmailApi.md#email_all_invoices_api_v1_billing_invoices_email_all_post) | **POST** /api/v1/billing/invoices/email-all | Email All Invoices
[**email_all_invoices_api_v1_billing_invoices_email_all_post_0**](BillingEmailApi.md#email_all_invoices_api_v1_billing_invoices_email_all_post_0) | **POST** /api/v1/billing/invoices/email-all | Email All Invoices
[**email_invoice_api_v1_billing_invoices_invoice_id_email_post**](BillingEmailApi.md#email_invoice_api_v1_billing_invoices_invoice_id_email_post) | **POST** /api/v1/billing/invoices/{invoice_id}/email | Email Invoice
[**email_invoice_api_v1_billing_invoices_invoice_id_email_post_0**](BillingEmailApi.md#email_invoice_api_v1_billing_invoices_invoice_id_email_post_0) | **POST** /api/v1/billing/invoices/{invoice_id}/email | Email Invoice


# **email_all_invoices_api_v1_billing_invoices_email_all_post**
> object email_all_invoices_api_v1_billing_invoices_email_all_post(body=body)

Email All Invoices

Email all invoices for the current organisation as a single ZIP of PDFs.
Body (optional): {"recipient_email": "...", "status_filters": [...], "date_from": "...", "date_to": "..."}

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
    api_instance = sensecore.BillingEmailApi(api_client)
    body = None # object |  (optional)

    try:
        # Email All Invoices
        api_response = api_instance.email_all_invoices_api_v1_billing_invoices_email_all_post(body=body)
        print("The response of BillingEmailApi->email_all_invoices_api_v1_billing_invoices_email_all_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingEmailApi->email_all_invoices_api_v1_billing_invoices_email_all_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | [optional] 

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

# **email_all_invoices_api_v1_billing_invoices_email_all_post_0**
> object email_all_invoices_api_v1_billing_invoices_email_all_post_0(body=body)

Email All Invoices

Email all invoices for the current organisation as a single ZIP of PDFs.
Body (optional): {"recipient_email": "...", "status_filters": [...], "date_from": "...", "date_to": "..."}

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
    api_instance = sensecore.BillingEmailApi(api_client)
    body = None # object |  (optional)

    try:
        # Email All Invoices
        api_response = api_instance.email_all_invoices_api_v1_billing_invoices_email_all_post_0(body=body)
        print("The response of BillingEmailApi->email_all_invoices_api_v1_billing_invoices_email_all_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingEmailApi->email_all_invoices_api_v1_billing_invoices_email_all_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | [optional] 

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

# **email_invoice_api_v1_billing_invoices_invoice_id_email_post**
> object email_invoice_api_v1_billing_invoices_invoice_id_email_post(invoice_id, body=body)

Email Invoice

Email a single invoice as PDF attachment.
Delegates to send_invoice_email() — same branded template as status-change emails.
Body (optional): {"recipient_email": "...", "cc_emails": ["..."], "message": "...", "copy_to_sender": true}

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
    api_instance = sensecore.BillingEmailApi(api_client)
    invoice_id = 'invoice_id_example' # str | Invoice ID or number
    body = None # object |  (optional)

    try:
        # Email Invoice
        api_response = api_instance.email_invoice_api_v1_billing_invoices_invoice_id_email_post(invoice_id, body=body)
        print("The response of BillingEmailApi->email_invoice_api_v1_billing_invoices_invoice_id_email_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingEmailApi->email_invoice_api_v1_billing_invoices_invoice_id_email_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**| Invoice ID or number | 
 **body** | **object**|  | [optional] 

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

# **email_invoice_api_v1_billing_invoices_invoice_id_email_post_0**
> object email_invoice_api_v1_billing_invoices_invoice_id_email_post_0(invoice_id, body=body)

Email Invoice

Email a single invoice as PDF attachment.
Delegates to send_invoice_email() — same branded template as status-change emails.
Body (optional): {"recipient_email": "...", "cc_emails": ["..."], "message": "...", "copy_to_sender": true}

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
    api_instance = sensecore.BillingEmailApi(api_client)
    invoice_id = 'invoice_id_example' # str | Invoice ID or number
    body = None # object |  (optional)

    try:
        # Email Invoice
        api_response = api_instance.email_invoice_api_v1_billing_invoices_invoice_id_email_post_0(invoice_id, body=body)
        print("The response of BillingEmailApi->email_invoice_api_v1_billing_invoices_invoice_id_email_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BillingEmailApi->email_invoice_api_v1_billing_invoices_invoice_id_email_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoice_id** | **str**| Invoice ID or number | 
 **body** | **object**|  | [optional] 

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

