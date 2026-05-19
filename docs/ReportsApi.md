# sensecore.ReportsApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**download_anomaly_pdf_api_v1_reports_anomaly_pdf_get**](ReportsApi.md#download_anomaly_pdf_api_v1_reports_anomaly_pdf_get) | **GET** /api/v1/reports/anomaly/pdf | Download Anomaly Pdf
[**download_carbon_pdf_api_v1_reports_carbon_pdf_get**](ReportsApi.md#download_carbon_pdf_api_v1_reports_carbon_pdf_get) | **GET** /api/v1/reports/carbon/pdf | Download Carbon Pdf
[**download_compliance_pdf_api_v1_reports_compliance_pdf_get**](ReportsApi.md#download_compliance_pdf_api_v1_reports_compliance_pdf_get) | **GET** /api/v1/reports/compliance/pdf | Download Compliance Pdf
[**download_portfolio_pdf_api_v1_reports_portfolio_pdf_get**](ReportsApi.md#download_portfolio_pdf_api_v1_reports_portfolio_pdf_get) | **GET** /api/v1/reports/portfolio/pdf | Download Portfolio Pdf


# **download_anomaly_pdf_api_v1_reports_anomaly_pdf_get**
> object download_anomaly_pdf_api_v1_reports_anomaly_pdf_get(period=period)

Download Anomaly Pdf

Generate anomaly detection report PDF.

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
    api_instance = sensecore.ReportsApi(api_client)
    period = 'Last 30 days' # str |  (optional) (default to 'Last 30 days')

    try:
        # Download Anomaly Pdf
        api_response = api_instance.download_anomaly_pdf_api_v1_reports_anomaly_pdf_get(period=period)
        print("The response of ReportsApi->download_anomaly_pdf_api_v1_reports_anomaly_pdf_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->download_anomaly_pdf_api_v1_reports_anomaly_pdf_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;Last 30 days&#39;]

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

# **download_carbon_pdf_api_v1_reports_carbon_pdf_get**
> object download_carbon_pdf_api_v1_reports_carbon_pdf_get(period=period, revenue_millions=revenue_millions, fte_count=fte_count, floor_area_m2=floor_area_m2)

Download Carbon Pdf

Generate SECR-compliant carbon report PDF.

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
    api_instance = sensecore.ReportsApi(api_client)
    period = '2025/26' # str |  (optional) (default to '2025/26')
    revenue_millions = 3.4 # float | Revenue in GBP millions (optional)
    fte_count = 56 # int | Full-time equivalent employees (optional)
    floor_area_m2 = 3.4 # float | Total floor area m2 (optional)

    try:
        # Download Carbon Pdf
        api_response = api_instance.download_carbon_pdf_api_v1_reports_carbon_pdf_get(period=period, revenue_millions=revenue_millions, fte_count=fte_count, floor_area_m2=floor_area_m2)
        print("The response of ReportsApi->download_carbon_pdf_api_v1_reports_carbon_pdf_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->download_carbon_pdf_api_v1_reports_carbon_pdf_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **period** | **str**|  | [optional] [default to &#39;2025/26&#39;]
 **revenue_millions** | **float**| Revenue in GBP millions | [optional] 
 **fte_count** | **int**| Full-time equivalent employees | [optional] 
 **floor_area_m2** | **float**| Total floor area m2 | [optional] 

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

# **download_compliance_pdf_api_v1_reports_compliance_pdf_get**
> object download_compliance_pdf_api_v1_reports_compliance_pdf_get()

Download Compliance Pdf

Generate multi-framework compliance status PDF.

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
    api_instance = sensecore.ReportsApi(api_client)

    try:
        # Download Compliance Pdf
        api_response = api_instance.download_compliance_pdf_api_v1_reports_compliance_pdf_get()
        print("The response of ReportsApi->download_compliance_pdf_api_v1_reports_compliance_pdf_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->download_compliance_pdf_api_v1_reports_compliance_pdf_get: %s\n" % e)
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

# **download_portfolio_pdf_api_v1_reports_portfolio_pdf_get**
> object download_portfolio_pdf_api_v1_reports_portfolio_pdf_get()

Download Portfolio Pdf

Generate portfolio performance report with CIBSE TM46 benchmarking.

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
    api_instance = sensecore.ReportsApi(api_client)

    try:
        # Download Portfolio Pdf
        api_response = api_instance.download_portfolio_pdf_api_v1_reports_portfolio_pdf_get()
        print("The response of ReportsApi->download_portfolio_pdf_api_v1_reports_portfolio_pdf_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ReportsApi->download_portfolio_pdf_api_v1_reports_portfolio_pdf_get: %s\n" % e)
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

