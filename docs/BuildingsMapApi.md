# sensecore.BuildingsMapApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**geocode_one_building_api_v1_buildings_building_id_geocode_post**](BuildingsMapApi.md#geocode_one_building_api_v1_buildings_building_id_geocode_post) | **POST** /api/v1/buildings/{building_id}/geocode | Geocode One Building
[**get_buildings_for_map_api_v1_buildings_map_get**](BuildingsMapApi.md#get_buildings_for_map_api_v1_buildings_map_get) | **GET** /api/v1/buildings/map | Get Buildings For Map


# **geocode_one_building_api_v1_buildings_building_id_geocode_post**
> object geocode_one_building_api_v1_buildings_building_id_geocode_post(building_id)

Geocode One Building

Force geocoding for one building. Useful when a postcode is added after
creation or an earlier geocoding attempt failed.

Auth: building must belong to the caller's org.

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
    api_instance = sensecore.BuildingsMapApi(api_client)
    building_id = 'building_id_example' # str | 

    try:
        # Geocode One Building
        api_response = api_instance.geocode_one_building_api_v1_buildings_building_id_geocode_post(building_id)
        print("The response of BuildingsMapApi->geocode_one_building_api_v1_buildings_building_id_geocode_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsMapApi->geocode_one_building_api_v1_buildings_building_id_geocode_post: %s\n" % e)
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

# **get_buildings_for_map_api_v1_buildings_map_get**
> object get_buildings_for_map_api_v1_buildings_map_get()

Get Buildings For Map

Return all mapped buildings for the current org with computed RAG status.

Response shape:
    {
      "portfolio_type": "Commercial Estate" | "Residential Portfolio",
      "summary": { total, red, amber, green, grey, mapped },
      "buildings": [
        { id, name, address, postcode, latitude, longitude,
          building_type, floor_area_m2, eui, benchmark_eui,
          annual_kwh, annual_cost_gbp, anomaly_count,
          energy_types, rag_status }
      ]
    }

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
    api_instance = sensecore.BuildingsMapApi(api_client)

    try:
        # Get Buildings For Map
        api_response = api_instance.get_buildings_for_map_api_v1_buildings_map_get()
        print("The response of BuildingsMapApi->get_buildings_for_map_api_v1_buildings_map_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling BuildingsMapApi->get_buildings_for_map_api_v1_buildings_map_get: %s\n" % e)
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

