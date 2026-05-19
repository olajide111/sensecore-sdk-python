# sensecore.BuildingsAdminApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**add_building_api_v1_admin_buildings_add_post**](BuildingsAdminApi.md#add_building_api_v1_admin_buildings_add_post) | **POST** /api/v1/admin/buildings/add | Add Building
[**add_building_api_v1_admin_buildings_add_post_0**](BuildingsAdminApi.md#add_building_api_v1_admin_buildings_add_post_0) | **POST** /api/v1/admin/buildings/add | Add Building
[**delete_building_api_v1_admin_buildings_delete_building_id_delete**](BuildingsAdminApi.md#delete_building_api_v1_admin_buildings_delete_building_id_delete) | **DELETE** /api/v1/admin/buildings/delete/{building_id} | Delete Building
[**delete_building_api_v1_admin_buildings_delete_building_id_delete_0**](BuildingsAdminApi.md#delete_building_api_v1_admin_buildings_delete_building_id_delete_0) | **DELETE** /api/v1/admin/buildings/delete/{building_id} | Delete Building
[**update_building_api_v1_admin_buildings_update_building_id_put**](BuildingsAdminApi.md#update_building_api_v1_admin_buildings_update_building_id_put) | **PUT** /api/v1/admin/buildings/update/{building_id} | Update Building
[**update_building_api_v1_admin_buildings_update_building_id_put_0**](BuildingsAdminApi.md#update_building_api_v1_admin_buildings_update_building_id_put_0) | **PUT** /api/v1/admin/buildings/update/{building_id} | Update Building


# **add_building_api_v1_admin_buildings_add_post**
> object add_building_api_v1_admin_buildings_add_post(body)

Add Building

Add a building. Body matches what the old direct-DB route used.

### Example


```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)


# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.BuildingsAdminApi(api_client)
    body = None # object | 

    try:
        # Add Building
        api_response = api_instance.add_building_api_v1_admin_buildings_add_post(body)
        print("The response of BuildingsAdminApi->add_building_api_v1_admin_buildings_add_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsAdminApi->add_building_api_v1_admin_buildings_add_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **add_building_api_v1_admin_buildings_add_post_0**
> object add_building_api_v1_admin_buildings_add_post_0(body)

Add Building

Add a building. Body matches what the old direct-DB route used.

### Example


```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)


# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.BuildingsAdminApi(api_client)
    body = None # object | 

    try:
        # Add Building
        api_response = api_instance.add_building_api_v1_admin_buildings_add_post_0(body)
        print("The response of BuildingsAdminApi->add_building_api_v1_admin_buildings_add_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsAdminApi->add_building_api_v1_admin_buildings_add_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_building_api_v1_admin_buildings_delete_building_id_delete**
> object delete_building_api_v1_admin_buildings_delete_building_id_delete(building_id)

Delete Building

Delete a building. Cascades remove meters via FK constraint.

### Example


```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)


# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.BuildingsAdminApi(api_client)
    building_id = 'building_id_example' # str | 

    try:
        # Delete Building
        api_response = api_instance.delete_building_api_v1_admin_buildings_delete_building_id_delete(building_id)
        print("The response of BuildingsAdminApi->delete_building_api_v1_admin_buildings_delete_building_id_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsAdminApi->delete_building_api_v1_admin_buildings_delete_building_id_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **str**|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_building_api_v1_admin_buildings_delete_building_id_delete_0**
> object delete_building_api_v1_admin_buildings_delete_building_id_delete_0(building_id)

Delete Building

Delete a building. Cascades remove meters via FK constraint.

### Example


```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)


# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.BuildingsAdminApi(api_client)
    building_id = 'building_id_example' # str | 

    try:
        # Delete Building
        api_response = api_instance.delete_building_api_v1_admin_buildings_delete_building_id_delete_0(building_id)
        print("The response of BuildingsAdminApi->delete_building_api_v1_admin_buildings_delete_building_id_delete_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsAdminApi->delete_building_api_v1_admin_buildings_delete_building_id_delete_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **str**|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_building_api_v1_admin_buildings_update_building_id_put**
> object update_building_api_v1_admin_buildings_update_building_id_put(building_id, body)

Update Building

Update fields on a building.

### Example


```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)


# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.BuildingsAdminApi(api_client)
    building_id = 'building_id_example' # str | 
    body = None # object | 

    try:
        # Update Building
        api_response = api_instance.update_building_api_v1_admin_buildings_update_building_id_put(building_id, body)
        print("The response of BuildingsAdminApi->update_building_api_v1_admin_buildings_update_building_id_put:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsAdminApi->update_building_api_v1_admin_buildings_update_building_id_put: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **str**|  | 
 **body** | **object**|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_building_api_v1_admin_buildings_update_building_id_put_0**
> object update_building_api_v1_admin_buildings_update_building_id_put_0(building_id, body)

Update Building

Update fields on a building.

### Example


```python
import sensecore
from sensecore.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.sensecoreai.com
# See configuration.py for a list of all supported configuration parameters.
configuration = sensecore.Configuration(
    host = "https://api.sensecoreai.com"
)


# Enter a context with an instance of the API client
with sensecore.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = sensecore.BuildingsAdminApi(api_client)
    building_id = 'building_id_example' # str | 
    body = None # object | 

    try:
        # Update Building
        api_response = api_instance.update_building_api_v1_admin_buildings_update_building_id_put_0(building_id, body)
        print("The response of BuildingsAdminApi->update_building_api_v1_admin_buildings_update_building_id_put_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsAdminApi->update_building_api_v1_admin_buildings_update_building_id_put_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **building_id** | **str**|  | 
 **body** | **object**|  | 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

