# sensecore.SavingsApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get**](SavingsApi.md#download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get) | **GET** /api/v1/savings/admin/{org_id}/pdf | Download Savings Pdf Admin
[**download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get_0**](SavingsApi.md#download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get_0) | **GET** /api/v1/savings/admin/{org_id}/pdf | Download Savings Pdf Admin
[**download_savings_pdf_api_v1_savings_pdf_get**](SavingsApi.md#download_savings_pdf_api_v1_savings_pdf_get) | **GET** /api/v1/savings/pdf | Download Savings Pdf
[**download_savings_pdf_api_v1_savings_pdf_get_0**](SavingsApi.md#download_savings_pdf_api_v1_savings_pdf_get_0) | **GET** /api/v1/savings/pdf | Download Savings Pdf
[**get_compliance_savings_api_v1_savings_compliance_get**](SavingsApi.md#get_compliance_savings_api_v1_savings_compliance_get) | **GET** /api/v1/savings/compliance | Get Compliance Savings
[**get_compliance_savings_api_v1_savings_compliance_get_0**](SavingsApi.md#get_compliance_savings_api_v1_savings_compliance_get_0) | **GET** /api/v1/savings/compliance | Get Compliance Savings
[**get_roi_metric_api_v1_savings_roi_get**](SavingsApi.md#get_roi_metric_api_v1_savings_roi_get) | **GET** /api/v1/savings/roi | Get Roi Metric
[**get_roi_metric_api_v1_savings_roi_get_0**](SavingsApi.md#get_roi_metric_api_v1_savings_roi_get_0) | **GET** /api/v1/savings/roi | Get Roi Metric
[**get_savings_by_building_api_v1_savings_buildings_get**](SavingsApi.md#get_savings_by_building_api_v1_savings_buildings_get) | **GET** /api/v1/savings/buildings | Get Savings By Building
[**get_savings_by_building_api_v1_savings_buildings_get_0**](SavingsApi.md#get_savings_by_building_api_v1_savings_buildings_get_0) | **GET** /api/v1/savings/buildings | Get Savings By Building
[**get_savings_for_org_api_v1_savings_admin_org_id_get**](SavingsApi.md#get_savings_for_org_api_v1_savings_admin_org_id_get) | **GET** /api/v1/savings/admin/{org_id} | Get Savings For Org
[**get_savings_for_org_api_v1_savings_admin_org_id_get_0**](SavingsApi.md#get_savings_for_org_api_v1_savings_admin_org_id_get_0) | **GET** /api/v1/savings/admin/{org_id} | Get Savings For Org
[**get_savings_summary_api_v1_savings_summary_get**](SavingsApi.md#get_savings_summary_api_v1_savings_summary_get) | **GET** /api/v1/savings/summary | Get Savings Summary
[**get_savings_summary_api_v1_savings_summary_get_0**](SavingsApi.md#get_savings_summary_api_v1_savings_summary_get_0) | **GET** /api/v1/savings/summary | Get Savings Summary
[**get_savings_trend_api_v1_savings_trend_get**](SavingsApi.md#get_savings_trend_api_v1_savings_trend_get) | **GET** /api/v1/savings/trend | Get Savings Trend
[**get_savings_trend_api_v1_savings_trend_get_0**](SavingsApi.md#get_savings_trend_api_v1_savings_trend_get_0) | **GET** /api/v1/savings/trend | Get Savings Trend


# **download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get**
> object download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get(org_id, period=period, start_date=start_date, end_date=end_date)

Download Savings Pdf Admin

Admin-only: Generate savings PDF for any organisation.

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
    api_instance = sensecore.SavingsApi(api_client)
    org_id = 56 # int | 
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Download Savings Pdf Admin
        api_response = api_instance.download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get(org_id, period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **int**|  | 
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get_0**
> object download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get_0(org_id, period=period, start_date=start_date, end_date=end_date)

Download Savings Pdf Admin

Admin-only: Generate savings PDF for any organisation.

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
    api_instance = sensecore.SavingsApi(api_client)
    org_id = 56 # int | 
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Download Savings Pdf Admin
        api_response = api_instance.download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get_0(org_id, period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->download_savings_pdf_admin_api_v1_savings_admin_org_id_pdf_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **int**|  | 
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **download_savings_pdf_api_v1_savings_pdf_get**
> object download_savings_pdf_api_v1_savings_pdf_get(period=period, start_date=start_date, end_date=end_date)

Download Savings Pdf

Generate and download a branded, board-ready savings PDF report.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Download Savings Pdf
        api_response = api_instance.download_savings_pdf_api_v1_savings_pdf_get(period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->download_savings_pdf_api_v1_savings_pdf_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->download_savings_pdf_api_v1_savings_pdf_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **download_savings_pdf_api_v1_savings_pdf_get_0**
> object download_savings_pdf_api_v1_savings_pdf_get_0(period=period, start_date=start_date, end_date=end_date)

Download Savings Pdf

Generate and download a branded, board-ready savings PDF report.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Download Savings Pdf
        api_response = api_instance.download_savings_pdf_api_v1_savings_pdf_get_0(period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->download_savings_pdf_api_v1_savings_pdf_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->download_savings_pdf_api_v1_savings_pdf_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **get_compliance_savings_api_v1_savings_compliance_get**
> object get_compliance_savings_api_v1_savings_compliance_get(period=period, start_date=start_date, end_date=end_date)

Get Compliance Savings

Compliance hours and cost savings breakdown by framework.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Get Compliance Savings
        api_response = api_instance.get_compliance_savings_api_v1_savings_compliance_get(period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->get_compliance_savings_api_v1_savings_compliance_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_compliance_savings_api_v1_savings_compliance_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **get_compliance_savings_api_v1_savings_compliance_get_0**
> object get_compliance_savings_api_v1_savings_compliance_get_0(period=period, start_date=start_date, end_date=end_date)

Get Compliance Savings

Compliance hours and cost savings breakdown by framework.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Get Compliance Savings
        api_response = api_instance.get_compliance_savings_api_v1_savings_compliance_get_0(period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->get_compliance_savings_api_v1_savings_compliance_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_compliance_savings_api_v1_savings_compliance_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **get_roi_metric_api_v1_savings_roi_get**
> object get_roi_metric_api_v1_savings_roi_get(period=period, start_date=start_date, end_date=end_date)

Get Roi Metric

ROI metric — savings vs subscription cost.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Get Roi Metric
        api_response = api_instance.get_roi_metric_api_v1_savings_roi_get(period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->get_roi_metric_api_v1_savings_roi_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_roi_metric_api_v1_savings_roi_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **get_roi_metric_api_v1_savings_roi_get_0**
> object get_roi_metric_api_v1_savings_roi_get_0(period=period, start_date=start_date, end_date=end_date)

Get Roi Metric

ROI metric — savings vs subscription cost.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Get Roi Metric
        api_response = api_instance.get_roi_metric_api_v1_savings_roi_get_0(period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->get_roi_metric_api_v1_savings_roi_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_roi_metric_api_v1_savings_roi_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **get_savings_by_building_api_v1_savings_buildings_get**
> object get_savings_by_building_api_v1_savings_buildings_get(period=period, start_date=start_date, end_date=end_date)

Get Savings By Building

Per-building savings breakdown, sorted by highest savings first.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Get Savings By Building
        api_response = api_instance.get_savings_by_building_api_v1_savings_buildings_get(period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->get_savings_by_building_api_v1_savings_buildings_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_savings_by_building_api_v1_savings_buildings_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **get_savings_by_building_api_v1_savings_buildings_get_0**
> object get_savings_by_building_api_v1_savings_buildings_get_0(period=period, start_date=start_date, end_date=end_date)

Get Savings By Building

Per-building savings breakdown, sorted by highest savings first.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Get Savings By Building
        api_response = api_instance.get_savings_by_building_api_v1_savings_buildings_get_0(period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->get_savings_by_building_api_v1_savings_buildings_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_savings_by_building_api_v1_savings_buildings_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **get_savings_for_org_api_v1_savings_admin_org_id_get**
> object get_savings_for_org_api_v1_savings_admin_org_id_get(org_id, period=period, start_date=start_date, end_date=end_date)

Get Savings For Org

Admin-only: full savings summary for any organisation.

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
    api_instance = sensecore.SavingsApi(api_client)
    org_id = 56 # int | 
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Get Savings For Org
        api_response = api_instance.get_savings_for_org_api_v1_savings_admin_org_id_get(org_id, period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->get_savings_for_org_api_v1_savings_admin_org_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_savings_for_org_api_v1_savings_admin_org_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **int**|  | 
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **get_savings_for_org_api_v1_savings_admin_org_id_get_0**
> object get_savings_for_org_api_v1_savings_admin_org_id_get_0(org_id, period=period, start_date=start_date, end_date=end_date)

Get Savings For Org

Admin-only: full savings summary for any organisation.

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
    api_instance = sensecore.SavingsApi(api_client)
    org_id = 56 # int | 
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Get Savings For Org
        api_response = api_instance.get_savings_for_org_api_v1_savings_admin_org_id_get_0(org_id, period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->get_savings_for_org_api_v1_savings_admin_org_id_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_savings_for_org_api_v1_savings_admin_org_id_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **org_id** | **int**|  | 
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **get_savings_summary_api_v1_savings_summary_get**
> object get_savings_summary_api_v1_savings_summary_get(period=period, start_date=start_date, end_date=end_date, building_ids=building_ids)

Get Savings Summary

Full savings summary for the logged-in user's organisation.
Returns all three pillars, ROI, per-building breakdown, and trend.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)
    building_ids = 'building_ids_example' # str | Comma-separated building IDs (optional)

    try:
        # Get Savings Summary
        api_response = api_instance.get_savings_summary_api_v1_savings_summary_get(period=period, start_date=start_date, end_date=end_date, building_ids=building_ids)
        print("The response of SavingsApi->get_savings_summary_api_v1_savings_summary_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_savings_summary_api_v1_savings_summary_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 
 **building_ids** | **str**| Comma-separated building IDs | [optional] 

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

# **get_savings_summary_api_v1_savings_summary_get_0**
> object get_savings_summary_api_v1_savings_summary_get_0(period=period, start_date=start_date, end_date=end_date, building_ids=building_ids)

Get Savings Summary

Full savings summary for the logged-in user's organisation.
Returns all three pillars, ROI, per-building breakdown, and trend.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)
    building_ids = 'building_ids_example' # str | Comma-separated building IDs (optional)

    try:
        # Get Savings Summary
        api_response = api_instance.get_savings_summary_api_v1_savings_summary_get_0(period=period, start_date=start_date, end_date=end_date, building_ids=building_ids)
        print("The response of SavingsApi->get_savings_summary_api_v1_savings_summary_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_savings_summary_api_v1_savings_summary_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 
 **building_ids** | **str**| Comma-separated building IDs | [optional] 

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

# **get_savings_trend_api_v1_savings_trend_get**
> object get_savings_trend_api_v1_savings_trend_get(period=period, start_date=start_date, end_date=end_date)

Get Savings Trend

Month-over-month savings trend data for charts.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Get Savings Trend
        api_response = api_instance.get_savings_trend_api_v1_savings_trend_get(period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->get_savings_trend_api_v1_savings_trend_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_savings_trend_api_v1_savings_trend_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

# **get_savings_trend_api_v1_savings_trend_get_0**
> object get_savings_trend_api_v1_savings_trend_get_0(period=period, start_date=start_date, end_date=end_date)

Get Savings Trend

Month-over-month savings trend data for charts.

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
    api_instance = sensecore.SavingsApi(api_client)
    period = 'quarterly' # str |  (optional) (default to 'quarterly')
    start_date = '2013-10-20' # date |  (optional)
    end_date = '2013-10-20' # date |  (optional)

    try:
        # Get Savings Trend
        api_response = api_instance.get_savings_trend_api_v1_savings_trend_get_0(period=period, start_date=start_date, end_date=end_date)
        print("The response of SavingsApi->get_savings_trend_api_v1_savings_trend_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling SavingsApi->get_savings_trend_api_v1_savings_trend_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;quarterly&#39;]
 **start_date** | **date**|  | [optional] 
 **end_date** | **date**|  | [optional] 

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

