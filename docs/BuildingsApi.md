# sensecore.BuildingsApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_meter_buildings_building_id_meters_post**](BuildingsApi.md#add_meter_buildings_building_id_meters_post) | **POST** /buildings/{building_id}/meters | Add Meter
[**bulk_upload_buildings_buildings_bulk_upload_post**](BuildingsApi.md#bulk_upload_buildings_buildings_bulk_upload_post) | **POST** /buildings/bulk-upload | Bulk Upload Buildings
[**create_building_api_v1_buildings_post**](BuildingsApi.md#create_building_api_v1_buildings_post) | **POST** /api/v1/buildings | Create Building
[**delete_building_api_v1_buildings_building_id_delete**](BuildingsApi.md#delete_building_api_v1_buildings_building_id_delete) | **DELETE** /api/v1/buildings/{building_id} | Delete Building
[**delete_meter_buildings_building_id_meters_meter_id_delete**](BuildingsApi.md#delete_meter_buildings_building_id_meters_meter_id_delete) | **DELETE** /buildings/{building_id}/meters/{meter_id} | Delete Meter
[**get_building_api_v1_buildings_building_id_get**](BuildingsApi.md#get_building_api_v1_buildings_building_id_get) | **GET** /api/v1/buildings/{building_id} | Get Building
[**get_building_buildings_building_id_get**](BuildingsApi.md#get_building_buildings_building_id_get) | **GET** /buildings/{building_id} | Get Building
[**get_meters_buildings_building_id_meters_get**](BuildingsApi.md#get_meters_buildings_building_id_meters_get) | **GET** /buildings/{building_id}/meters | Get Meters
[**list_buildings_api_v1_buildings_get**](BuildingsApi.md#list_buildings_api_v1_buildings_get) | **GET** /api/v1/buildings | List Buildings
[**update_building_api_v1_buildings_building_id_patch**](BuildingsApi.md#update_building_api_v1_buildings_building_id_patch) | **PATCH** /api/v1/buildings/{building_id} | Update Building
[**update_meter_buildings_building_id_meters_meter_id_patch**](BuildingsApi.md#update_meter_buildings_building_id_meters_meter_id_patch) | **PATCH** /buildings/{building_id}/meters/{meter_id} | Update Meter


# **add_meter_buildings_building_id_meters_post**
> object add_meter_buildings_building_id_meters_post(building_id, body)

Add Meter

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
    api_instance = sensecore.BuildingsApi(api_client)
    building_id = 'building_id_example' # str | 
    body = None # object | 

    try:
        # Add Meter
        api_response = api_instance.add_meter_buildings_building_id_meters_post(building_id, body)
        print("The response of BuildingsApi->add_meter_buildings_building_id_meters_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsApi->add_meter_buildings_building_id_meters_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **str**|  | 
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

# **bulk_upload_buildings_buildings_bulk_upload_post**
> object bulk_upload_buildings_buildings_bulk_upload_post(body)

Bulk Upload Buildings

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
    api_instance = sensecore.BuildingsApi(api_client)
    body = None # object | 

    try:
        # Bulk Upload Buildings
        api_response = api_instance.bulk_upload_buildings_buildings_bulk_upload_post(body)
        print("The response of BuildingsApi->bulk_upload_buildings_buildings_bulk_upload_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsApi->bulk_upload_buildings_buildings_bulk_upload_post: %s\n" % e)
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

# **create_building_api_v1_buildings_post**
> object create_building_api_v1_buildings_post(body)

Create Building

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
    api_instance = sensecore.BuildingsApi(api_client)
    body = None # object | 

    try:
        # Create Building
        api_response = api_instance.create_building_api_v1_buildings_post(body)
        print("The response of BuildingsApi->create_building_api_v1_buildings_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsApi->create_building_api_v1_buildings_post: %s\n" % e)
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

# **delete_building_api_v1_buildings_building_id_delete**
> object delete_building_api_v1_buildings_building_id_delete(building_id)

Delete Building

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
    api_instance = sensecore.BuildingsApi(api_client)
    building_id = 56 # int | 

    try:
        # Delete Building
        api_response = api_instance.delete_building_api_v1_buildings_building_id_delete(building_id)
        print("The response of BuildingsApi->delete_building_api_v1_buildings_building_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsApi->delete_building_api_v1_buildings_building_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **int**|  | 

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

# **delete_meter_buildings_building_id_meters_meter_id_delete**
> object delete_meter_buildings_building_id_meters_meter_id_delete(building_id, meter_id)

Delete Meter

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
    api_instance = sensecore.BuildingsApi(api_client)
    building_id = 'building_id_example' # str | 
    meter_id = 'meter_id_example' # str | 

    try:
        # Delete Meter
        api_response = api_instance.delete_meter_buildings_building_id_meters_meter_id_delete(building_id, meter_id)
        print("The response of BuildingsApi->delete_meter_buildings_building_id_meters_meter_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsApi->delete_meter_buildings_building_id_meters_meter_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **str**|  | 
 **meter_id** | **str**|  | 

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

# **get_building_api_v1_buildings_building_id_get**
> object get_building_api_v1_buildings_building_id_get(building_id)

Get Building

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
    api_instance = sensecore.BuildingsApi(api_client)
    building_id = 56 # int | 

    try:
        # Get Building
        api_response = api_instance.get_building_api_v1_buildings_building_id_get(building_id)
        print("The response of BuildingsApi->get_building_api_v1_buildings_building_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsApi->get_building_api_v1_buildings_building_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **int**|  | 

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

# **get_building_buildings_building_id_get**
> object get_building_buildings_building_id_get(building_id)

Get Building

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
    api_instance = sensecore.BuildingsApi(api_client)
    building_id = 'building_id_example' # str | 

    try:
        # Get Building
        api_response = api_instance.get_building_buildings_building_id_get(building_id)
        print("The response of BuildingsApi->get_building_buildings_building_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsApi->get_building_buildings_building_id_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **str**|  | 

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

# **get_meters_buildings_building_id_meters_get**
> object get_meters_buildings_building_id_meters_get(building_id)

Get Meters

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
    api_instance = sensecore.BuildingsApi(api_client)
    building_id = 'building_id_example' # str | 

    try:
        # Get Meters
        api_response = api_instance.get_meters_buildings_building_id_meters_get(building_id)
        print("The response of BuildingsApi->get_meters_buildings_building_id_meters_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsApi->get_meters_buildings_building_id_meters_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **str**|  | 

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

# **list_buildings_api_v1_buildings_get**
> object list_buildings_api_v1_buildings_get()

List Buildings

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
    api_instance = sensecore.BuildingsApi(api_client)

    try:
        # List Buildings
        api_response = api_instance.list_buildings_api_v1_buildings_get()
        print("The response of BuildingsApi->list_buildings_api_v1_buildings_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsApi->list_buildings_api_v1_buildings_get: %s\n" % e)
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

# **update_building_api_v1_buildings_building_id_patch**
> object update_building_api_v1_buildings_building_id_patch(building_id, body)

Update Building

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
    api_instance = sensecore.BuildingsApi(api_client)
    building_id = 56 # int | 
    body = None # object | 

    try:
        # Update Building
        api_response = api_instance.update_building_api_v1_buildings_building_id_patch(building_id, body)
        print("The response of BuildingsApi->update_building_api_v1_buildings_building_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsApi->update_building_api_v1_buildings_building_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **int**|  | 
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

# **update_meter_buildings_building_id_meters_meter_id_patch**
> object update_meter_buildings_building_id_meters_meter_id_patch(building_id, meter_id, body)

Update Meter

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
    api_instance = sensecore.BuildingsApi(api_client)
    building_id = 'building_id_example' # str | 
    meter_id = 'meter_id_example' # str | 
    body = None # object | 

    try:
        # Update Meter
        api_response = api_instance.update_meter_buildings_building_id_meters_meter_id_patch(building_id, meter_id, body)
        print("The response of BuildingsApi->update_meter_buildings_building_id_meters_meter_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsApi->update_meter_buildings_building_id_meters_meter_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **str**|  | 
 **meter_id** | **str**|  | 
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

