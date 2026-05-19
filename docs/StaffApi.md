# sensecore.StaffApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_staff_api_v1_admin_staff_post**](StaffApi.md#create_staff_api_v1_admin_staff_post) | **POST** /api/v1/admin/staff | Create Staff
[**create_staff_api_v1_admin_staff_post_0**](StaffApi.md#create_staff_api_v1_admin_staff_post_0) | **POST** /api/v1/admin/staff | Create Staff
[**delete_staff_api_v1_admin_staff_sid_delete**](StaffApi.md#delete_staff_api_v1_admin_staff_sid_delete) | **DELETE** /api/v1/admin/staff/{sid} | Delete Staff
[**delete_staff_api_v1_admin_staff_sid_delete_0**](StaffApi.md#delete_staff_api_v1_admin_staff_sid_delete_0) | **DELETE** /api/v1/admin/staff/{sid} | Delete Staff
[**get_activity_api_v1_admin_staff_sid_activity_get**](StaffApi.md#get_activity_api_v1_admin_staff_sid_activity_get) | **GET** /api/v1/admin/staff/{sid}/activity | Get Activity
[**get_activity_api_v1_admin_staff_sid_activity_get_0**](StaffApi.md#get_activity_api_v1_admin_staff_sid_activity_get_0) | **GET** /api/v1/admin/staff/{sid}/activity | Get Activity
[**get_sessions_api_v1_admin_staff_sid_sessions_get**](StaffApi.md#get_sessions_api_v1_admin_staff_sid_sessions_get) | **GET** /api/v1/admin/staff/{sid}/sessions | Get Sessions
[**get_sessions_api_v1_admin_staff_sid_sessions_get_0**](StaffApi.md#get_sessions_api_v1_admin_staff_sid_sessions_get_0) | **GET** /api/v1/admin/staff/{sid}/sessions | Get Sessions
[**get_staff_api_v1_admin_staff_sid_get**](StaffApi.md#get_staff_api_v1_admin_staff_sid_get) | **GET** /api/v1/admin/staff/{sid} | Get Staff
[**get_staff_api_v1_admin_staff_sid_get_0**](StaffApi.md#get_staff_api_v1_admin_staff_sid_get_0) | **GET** /api/v1/admin/staff/{sid} | Get Staff
[**heartbeat_api_v1_admin_staff_heartbeat_post**](StaffApi.md#heartbeat_api_v1_admin_staff_heartbeat_post) | **POST** /api/v1/admin/staff/heartbeat | Heartbeat
[**heartbeat_api_v1_admin_staff_heartbeat_post_0**](StaffApi.md#heartbeat_api_v1_admin_staff_heartbeat_post_0) | **POST** /api/v1/admin/staff/heartbeat | Heartbeat
[**list_roles_api_v1_admin_staff_roles_list_get**](StaffApi.md#list_roles_api_v1_admin_staff_roles_list_get) | **GET** /api/v1/admin/staff/roles/list | List Roles
[**list_roles_api_v1_admin_staff_roles_list_get_0**](StaffApi.md#list_roles_api_v1_admin_staff_roles_list_get_0) | **GET** /api/v1/admin/staff/roles/list | List Roles
[**list_staff_api_v1_admin_staff_get**](StaffApi.md#list_staff_api_v1_admin_staff_get) | **GET** /api/v1/admin/staff | List Staff
[**list_staff_api_v1_admin_staff_get_0**](StaffApi.md#list_staff_api_v1_admin_staff_get_0) | **GET** /api/v1/admin/staff | List Staff
[**login_event_api_v1_admin_staff_login_event_post**](StaffApi.md#login_event_api_v1_admin_staff_login_event_post) | **POST** /api/v1/admin/staff/login-event | Login Event
[**login_event_api_v1_admin_staff_login_event_post_0**](StaffApi.md#login_event_api_v1_admin_staff_login_event_post_0) | **POST** /api/v1/admin/staff/login-event | Login Event
[**logout_event_api_v1_admin_staff_logout_event_post**](StaffApi.md#logout_event_api_v1_admin_staff_logout_event_post) | **POST** /api/v1/admin/staff/logout-event | Logout Event
[**logout_event_api_v1_admin_staff_logout_event_post_0**](StaffApi.md#logout_event_api_v1_admin_staff_logout_event_post_0) | **POST** /api/v1/admin/staff/logout-event | Logout Event
[**update_staff_api_v1_admin_staff_sid_patch**](StaffApi.md#update_staff_api_v1_admin_staff_sid_patch) | **PATCH** /api/v1/admin/staff/{sid} | Update Staff
[**update_staff_api_v1_admin_staff_sid_patch_0**](StaffApi.md#update_staff_api_v1_admin_staff_sid_patch_0) | **PATCH** /api/v1/admin/staff/{sid} | Update Staff
[**upload_avatar_api_v1_admin_staff_sid_avatar_post**](StaffApi.md#upload_avatar_api_v1_admin_staff_sid_avatar_post) | **POST** /api/v1/admin/staff/{sid}/avatar | Upload Avatar
[**upload_avatar_api_v1_admin_staff_sid_avatar_post_0**](StaffApi.md#upload_avatar_api_v1_admin_staff_sid_avatar_post_0) | **POST** /api/v1/admin/staff/{sid}/avatar | Upload Avatar


# **create_staff_api_v1_admin_staff_post**
> object create_staff_api_v1_admin_staff_post(body)

Create Staff

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
    api_instance = sensecore.StaffApi(api_client)
    body = None # object | 

    try:
        # Create Staff
        api_response = api_instance.create_staff_api_v1_admin_staff_post(body)
        print("The response of StaffApi->create_staff_api_v1_admin_staff_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->create_staff_api_v1_admin_staff_post: %s\n" % e)
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

# **create_staff_api_v1_admin_staff_post_0**
> object create_staff_api_v1_admin_staff_post_0(body)

Create Staff

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
    api_instance = sensecore.StaffApi(api_client)
    body = None # object | 

    try:
        # Create Staff
        api_response = api_instance.create_staff_api_v1_admin_staff_post_0(body)
        print("The response of StaffApi->create_staff_api_v1_admin_staff_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->create_staff_api_v1_admin_staff_post_0: %s\n" % e)
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

# **delete_staff_api_v1_admin_staff_sid_delete**
> object delete_staff_api_v1_admin_staff_sid_delete(sid)

Delete Staff

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 

    try:
        # Delete Staff
        api_response = api_instance.delete_staff_api_v1_admin_staff_sid_delete(sid)
        print("The response of StaffApi->delete_staff_api_v1_admin_staff_sid_delete:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->delete_staff_api_v1_admin_staff_sid_delete: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 

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

# **delete_staff_api_v1_admin_staff_sid_delete_0**
> object delete_staff_api_v1_admin_staff_sid_delete_0(sid)

Delete Staff

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 

    try:
        # Delete Staff
        api_response = api_instance.delete_staff_api_v1_admin_staff_sid_delete_0(sid)
        print("The response of StaffApi->delete_staff_api_v1_admin_staff_sid_delete_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->delete_staff_api_v1_admin_staff_sid_delete_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 

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

# **get_activity_api_v1_admin_staff_sid_activity_get**
> object get_activity_api_v1_admin_staff_sid_activity_get(sid)

Get Activity

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 

    try:
        # Get Activity
        api_response = api_instance.get_activity_api_v1_admin_staff_sid_activity_get(sid)
        print("The response of StaffApi->get_activity_api_v1_admin_staff_sid_activity_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->get_activity_api_v1_admin_staff_sid_activity_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 

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

# **get_activity_api_v1_admin_staff_sid_activity_get_0**
> object get_activity_api_v1_admin_staff_sid_activity_get_0(sid)

Get Activity

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 

    try:
        # Get Activity
        api_response = api_instance.get_activity_api_v1_admin_staff_sid_activity_get_0(sid)
        print("The response of StaffApi->get_activity_api_v1_admin_staff_sid_activity_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->get_activity_api_v1_admin_staff_sid_activity_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 

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

# **get_sessions_api_v1_admin_staff_sid_sessions_get**
> object get_sessions_api_v1_admin_staff_sid_sessions_get(sid)

Get Sessions

Get login session history for a staff member.

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 

    try:
        # Get Sessions
        api_response = api_instance.get_sessions_api_v1_admin_staff_sid_sessions_get(sid)
        print("The response of StaffApi->get_sessions_api_v1_admin_staff_sid_sessions_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->get_sessions_api_v1_admin_staff_sid_sessions_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 

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

# **get_sessions_api_v1_admin_staff_sid_sessions_get_0**
> object get_sessions_api_v1_admin_staff_sid_sessions_get_0(sid)

Get Sessions

Get login session history for a staff member.

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 

    try:
        # Get Sessions
        api_response = api_instance.get_sessions_api_v1_admin_staff_sid_sessions_get_0(sid)
        print("The response of StaffApi->get_sessions_api_v1_admin_staff_sid_sessions_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->get_sessions_api_v1_admin_staff_sid_sessions_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 

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

# **get_staff_api_v1_admin_staff_sid_get**
> object get_staff_api_v1_admin_staff_sid_get(sid)

Get Staff

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 

    try:
        # Get Staff
        api_response = api_instance.get_staff_api_v1_admin_staff_sid_get(sid)
        print("The response of StaffApi->get_staff_api_v1_admin_staff_sid_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->get_staff_api_v1_admin_staff_sid_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 

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

# **get_staff_api_v1_admin_staff_sid_get_0**
> object get_staff_api_v1_admin_staff_sid_get_0(sid)

Get Staff

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 

    try:
        # Get Staff
        api_response = api_instance.get_staff_api_v1_admin_staff_sid_get_0(sid)
        print("The response of StaffApi->get_staff_api_v1_admin_staff_sid_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->get_staff_api_v1_admin_staff_sid_get_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 

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

# **heartbeat_api_v1_admin_staff_heartbeat_post**
> object heartbeat_api_v1_admin_staff_heartbeat_post(body=body)

Heartbeat

Update last_active. Decodes JWT directly, no FastAPI auth dep.

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
    api_instance = sensecore.StaffApi(api_client)
    body = None # object |  (optional)

    try:
        # Heartbeat
        api_response = api_instance.heartbeat_api_v1_admin_staff_heartbeat_post(body=body)
        print("The response of StaffApi->heartbeat_api_v1_admin_staff_heartbeat_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->heartbeat_api_v1_admin_staff_heartbeat_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | [optional] 

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

# **heartbeat_api_v1_admin_staff_heartbeat_post_0**
> object heartbeat_api_v1_admin_staff_heartbeat_post_0(body=body)

Heartbeat

Update last_active. Decodes JWT directly, no FastAPI auth dep.

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
    api_instance = sensecore.StaffApi(api_client)
    body = None # object |  (optional)

    try:
        # Heartbeat
        api_response = api_instance.heartbeat_api_v1_admin_staff_heartbeat_post_0(body=body)
        print("The response of StaffApi->heartbeat_api_v1_admin_staff_heartbeat_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->heartbeat_api_v1_admin_staff_heartbeat_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | [optional] 

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

# **list_roles_api_v1_admin_staff_roles_list_get**
> object list_roles_api_v1_admin_staff_roles_list_get()

List Roles

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
    api_instance = sensecore.StaffApi(api_client)

    try:
        # List Roles
        api_response = api_instance.list_roles_api_v1_admin_staff_roles_list_get()
        print("The response of StaffApi->list_roles_api_v1_admin_staff_roles_list_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->list_roles_api_v1_admin_staff_roles_list_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_roles_api_v1_admin_staff_roles_list_get_0**
> object list_roles_api_v1_admin_staff_roles_list_get_0()

List Roles

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
    api_instance = sensecore.StaffApi(api_client)

    try:
        # List Roles
        api_response = api_instance.list_roles_api_v1_admin_staff_roles_list_get_0()
        print("The response of StaffApi->list_roles_api_v1_admin_staff_roles_list_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->list_roles_api_v1_admin_staff_roles_list_get_0: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_staff_api_v1_admin_staff_get**
> object list_staff_api_v1_admin_staff_get()

List Staff

List all staff with current online status.

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
    api_instance = sensecore.StaffApi(api_client)

    try:
        # List Staff
        api_response = api_instance.list_staff_api_v1_admin_staff_get()
        print("The response of StaffApi->list_staff_api_v1_admin_staff_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->list_staff_api_v1_admin_staff_get: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **list_staff_api_v1_admin_staff_get_0**
> object list_staff_api_v1_admin_staff_get_0()

List Staff

List all staff with current online status.

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
    api_instance = sensecore.StaffApi(api_client)

    try:
        # List Staff
        api_response = api_instance.list_staff_api_v1_admin_staff_get_0()
        print("The response of StaffApi->list_staff_api_v1_admin_staff_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->list_staff_api_v1_admin_staff_get_0: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **login_event_api_v1_admin_staff_login_event_post**
> object login_event_api_v1_admin_staff_login_event_post(body=body)

Login Event

Record a new login session.

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
    api_instance = sensecore.StaffApi(api_client)
    body = None # object |  (optional)

    try:
        # Login Event
        api_response = api_instance.login_event_api_v1_admin_staff_login_event_post(body=body)
        print("The response of StaffApi->login_event_api_v1_admin_staff_login_event_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->login_event_api_v1_admin_staff_login_event_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | [optional] 

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

# **login_event_api_v1_admin_staff_login_event_post_0**
> object login_event_api_v1_admin_staff_login_event_post_0(body=body)

Login Event

Record a new login session.

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
    api_instance = sensecore.StaffApi(api_client)
    body = None # object |  (optional)

    try:
        # Login Event
        api_response = api_instance.login_event_api_v1_admin_staff_login_event_post_0(body=body)
        print("The response of StaffApi->login_event_api_v1_admin_staff_login_event_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->login_event_api_v1_admin_staff_login_event_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **object**|  | [optional] 

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

# **logout_event_api_v1_admin_staff_logout_event_post**
> object logout_event_api_v1_admin_staff_logout_event_post()

Logout Event

Close active session.

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
    api_instance = sensecore.StaffApi(api_client)

    try:
        # Logout Event
        api_response = api_instance.logout_event_api_v1_admin_staff_logout_event_post()
        print("The response of StaffApi->logout_event_api_v1_admin_staff_logout_event_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->logout_event_api_v1_admin_staff_logout_event_post: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **logout_event_api_v1_admin_staff_logout_event_post_0**
> object logout_event_api_v1_admin_staff_logout_event_post_0()

Logout Event

Close active session.

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
    api_instance = sensecore.StaffApi(api_client)

    try:
        # Logout Event
        api_response = api_instance.logout_event_api_v1_admin_staff_logout_event_post_0()
        print("The response of StaffApi->logout_event_api_v1_admin_staff_logout_event_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->logout_event_api_v1_admin_staff_logout_event_post_0: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_staff_api_v1_admin_staff_sid_patch**
> object update_staff_api_v1_admin_staff_sid_patch(sid, body)

Update Staff

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 
    body = None # object | 

    try:
        # Update Staff
        api_response = api_instance.update_staff_api_v1_admin_staff_sid_patch(sid, body)
        print("The response of StaffApi->update_staff_api_v1_admin_staff_sid_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->update_staff_api_v1_admin_staff_sid_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 
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

# **update_staff_api_v1_admin_staff_sid_patch_0**
> object update_staff_api_v1_admin_staff_sid_patch_0(sid, body)

Update Staff

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 
    body = None # object | 

    try:
        # Update Staff
        api_response = api_instance.update_staff_api_v1_admin_staff_sid_patch_0(sid, body)
        print("The response of StaffApi->update_staff_api_v1_admin_staff_sid_patch_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->update_staff_api_v1_admin_staff_sid_patch_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 
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

# **upload_avatar_api_v1_admin_staff_sid_avatar_post**
> object upload_avatar_api_v1_admin_staff_sid_avatar_post(sid, body)

Upload Avatar

Upload avatar as base64 data URL. Max 500KB.

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 
    body = None # object | 

    try:
        # Upload Avatar
        api_response = api_instance.upload_avatar_api_v1_admin_staff_sid_avatar_post(sid, body)
        print("The response of StaffApi->upload_avatar_api_v1_admin_staff_sid_avatar_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->upload_avatar_api_v1_admin_staff_sid_avatar_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 
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

# **upload_avatar_api_v1_admin_staff_sid_avatar_post_0**
> object upload_avatar_api_v1_admin_staff_sid_avatar_post_0(sid, body)

Upload Avatar

Upload avatar as base64 data URL. Max 500KB.

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
    api_instance = sensecore.StaffApi(api_client)
    sid = 'sid_example' # str | 
    body = None # object | 

    try:
        # Upload Avatar
        api_response = api_instance.upload_avatar_api_v1_admin_staff_sid_avatar_post_0(sid, body)
        print("The response of StaffApi->upload_avatar_api_v1_admin_staff_sid_avatar_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StaffApi->upload_avatar_api_v1_admin_staff_sid_avatar_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sid** | **str**|  | 
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

