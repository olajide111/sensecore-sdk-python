# sensecore.RolesApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**change_user_role_api_v1_admin_roles_users_user_id_role_patch**](RolesApi.md#change_user_role_api_v1_admin_roles_users_user_id_role_patch) | **PATCH** /api/v1/admin/roles/users/{user_id}/role | Change User Role
[**change_user_role_api_v1_admin_roles_users_user_id_role_patch_0**](RolesApi.md#change_user_role_api_v1_admin_roles_users_user_id_role_patch_0) | **PATCH** /api/v1/admin/roles/users/{user_id}/role | Change User Role
[**get_my_permissions_api_v1_admin_roles_my_permissions_get**](RolesApi.md#get_my_permissions_api_v1_admin_roles_my_permissions_get) | **GET** /api/v1/admin/roles/my-permissions | Get My Permissions
[**get_my_permissions_api_v1_admin_roles_my_permissions_get_0**](RolesApi.md#get_my_permissions_api_v1_admin_roles_my_permissions_get_0) | **GET** /api/v1/admin/roles/my-permissions | Get My Permissions
[**get_role_definitions_api_v1_admin_roles_definitions_get**](RolesApi.md#get_role_definitions_api_v1_admin_roles_definitions_get) | **GET** /api/v1/admin/roles/definitions | Get Role Definitions
[**get_role_definitions_api_v1_admin_roles_definitions_get_0**](RolesApi.md#get_role_definitions_api_v1_admin_roles_definitions_get_0) | **GET** /api/v1/admin/roles/definitions | Get Role Definitions
[**get_users_with_roles_api_v1_admin_roles_users_get**](RolesApi.md#get_users_with_roles_api_v1_admin_roles_users_get) | **GET** /api/v1/admin/roles/users | Get Users With Roles
[**get_users_with_roles_api_v1_admin_roles_users_get_0**](RolesApi.md#get_users_with_roles_api_v1_admin_roles_users_get_0) | **GET** /api/v1/admin/roles/users | Get Users With Roles
[**reset_permissions_api_v1_admin_roles_users_user_id_reset_post**](RolesApi.md#reset_permissions_api_v1_admin_roles_users_user_id_reset_post) | **POST** /api/v1/admin/roles/users/{user_id}/reset | Reset Permissions
[**reset_permissions_api_v1_admin_roles_users_user_id_reset_post_0**](RolesApi.md#reset_permissions_api_v1_admin_roles_users_user_id_reset_post_0) | **POST** /api/v1/admin/roles/users/{user_id}/reset | Reset Permissions
[**update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch**](RolesApi.md#update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch) | **PATCH** /api/v1/admin/roles/users/{user_id}/permissions | Update User Permissions
[**update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch_0**](RolesApi.md#update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch_0) | **PATCH** /api/v1/admin/roles/users/{user_id}/permissions | Update User Permissions


# **change_user_role_api_v1_admin_roles_users_user_id_role_patch**
> object change_user_role_api_v1_admin_roles_users_user_id_role_patch(user_id, body)

Change User Role

Change a user role and reset permissions to role defaults.

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
    api_instance = sensecore.RolesApi(api_client)
    user_id = 'user_id_example' # str | 
    body = None # object | 

    try:
        # Change User Role
        api_response = api_instance.change_user_role_api_v1_admin_roles_users_user_id_role_patch(user_id, body)
        print("The response of RolesApi->change_user_role_api_v1_admin_roles_users_user_id_role_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->change_user_role_api_v1_admin_roles_users_user_id_role_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **str**|  | 
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

# **change_user_role_api_v1_admin_roles_users_user_id_role_patch_0**
> object change_user_role_api_v1_admin_roles_users_user_id_role_patch_0(user_id, body)

Change User Role

Change a user role and reset permissions to role defaults.

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
    api_instance = sensecore.RolesApi(api_client)
    user_id = 'user_id_example' # str | 
    body = None # object | 

    try:
        # Change User Role
        api_response = api_instance.change_user_role_api_v1_admin_roles_users_user_id_role_patch_0(user_id, body)
        print("The response of RolesApi->change_user_role_api_v1_admin_roles_users_user_id_role_patch_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->change_user_role_api_v1_admin_roles_users_user_id_role_patch_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **str**|  | 
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

# **get_my_permissions_api_v1_admin_roles_my_permissions_get**
> object get_my_permissions_api_v1_admin_roles_my_permissions_get()

Get My Permissions

Get the current user permissions (for frontend gating).

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
    api_instance = sensecore.RolesApi(api_client)

    try:
        # Get My Permissions
        api_response = api_instance.get_my_permissions_api_v1_admin_roles_my_permissions_get()
        print("The response of RolesApi->get_my_permissions_api_v1_admin_roles_my_permissions_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->get_my_permissions_api_v1_admin_roles_my_permissions_get: %s\n" % e)
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

# **get_my_permissions_api_v1_admin_roles_my_permissions_get_0**
> object get_my_permissions_api_v1_admin_roles_my_permissions_get_0()

Get My Permissions

Get the current user permissions (for frontend gating).

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
    api_instance = sensecore.RolesApi(api_client)

    try:
        # Get My Permissions
        api_response = api_instance.get_my_permissions_api_v1_admin_roles_my_permissions_get_0()
        print("The response of RolesApi->get_my_permissions_api_v1_admin_roles_my_permissions_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->get_my_permissions_api_v1_admin_roles_my_permissions_get_0: %s\n" % e)
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

# **get_role_definitions_api_v1_admin_roles_definitions_get**
> object get_role_definitions_api_v1_admin_roles_definitions_get()

Get Role Definitions

Return all role definitions with their default permissions.

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
    api_instance = sensecore.RolesApi(api_client)

    try:
        # Get Role Definitions
        api_response = api_instance.get_role_definitions_api_v1_admin_roles_definitions_get()
        print("The response of RolesApi->get_role_definitions_api_v1_admin_roles_definitions_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->get_role_definitions_api_v1_admin_roles_definitions_get: %s\n" % e)
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

# **get_role_definitions_api_v1_admin_roles_definitions_get_0**
> object get_role_definitions_api_v1_admin_roles_definitions_get_0()

Get Role Definitions

Return all role definitions with their default permissions.

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
    api_instance = sensecore.RolesApi(api_client)

    try:
        # Get Role Definitions
        api_response = api_instance.get_role_definitions_api_v1_admin_roles_definitions_get_0()
        print("The response of RolesApi->get_role_definitions_api_v1_admin_roles_definitions_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->get_role_definitions_api_v1_admin_roles_definitions_get_0: %s\n" % e)
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

# **get_users_with_roles_api_v1_admin_roles_users_get**
> object get_users_with_roles_api_v1_admin_roles_users_get()

Get Users With Roles

List all users with their roles and permission summary.

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
    api_instance = sensecore.RolesApi(api_client)

    try:
        # Get Users With Roles
        api_response = api_instance.get_users_with_roles_api_v1_admin_roles_users_get()
        print("The response of RolesApi->get_users_with_roles_api_v1_admin_roles_users_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->get_users_with_roles_api_v1_admin_roles_users_get: %s\n" % e)
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

# **get_users_with_roles_api_v1_admin_roles_users_get_0**
> object get_users_with_roles_api_v1_admin_roles_users_get_0()

Get Users With Roles

List all users with their roles and permission summary.

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
    api_instance = sensecore.RolesApi(api_client)

    try:
        # Get Users With Roles
        api_response = api_instance.get_users_with_roles_api_v1_admin_roles_users_get_0()
        print("The response of RolesApi->get_users_with_roles_api_v1_admin_roles_users_get_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->get_users_with_roles_api_v1_admin_roles_users_get_0: %s\n" % e)
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

# **reset_permissions_api_v1_admin_roles_users_user_id_reset_post**
> object reset_permissions_api_v1_admin_roles_users_user_id_reset_post(user_id)

Reset Permissions

Reset user permissions back to their role defaults.

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
    api_instance = sensecore.RolesApi(api_client)
    user_id = 'user_id_example' # str | 

    try:
        # Reset Permissions
        api_response = api_instance.reset_permissions_api_v1_admin_roles_users_user_id_reset_post(user_id)
        print("The response of RolesApi->reset_permissions_api_v1_admin_roles_users_user_id_reset_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->reset_permissions_api_v1_admin_roles_users_user_id_reset_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **str**|  | 

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

# **reset_permissions_api_v1_admin_roles_users_user_id_reset_post_0**
> object reset_permissions_api_v1_admin_roles_users_user_id_reset_post_0(user_id)

Reset Permissions

Reset user permissions back to their role defaults.

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
    api_instance = sensecore.RolesApi(api_client)
    user_id = 'user_id_example' # str | 

    try:
        # Reset Permissions
        api_response = api_instance.reset_permissions_api_v1_admin_roles_users_user_id_reset_post_0(user_id)
        print("The response of RolesApi->reset_permissions_api_v1_admin_roles_users_user_id_reset_post_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->reset_permissions_api_v1_admin_roles_users_user_id_reset_post_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **str**|  | 

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

# **update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch**
> object update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch(user_id, body)

Update User Permissions

Update individual permissions for a user (custom override).

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
    api_instance = sensecore.RolesApi(api_client)
    user_id = 'user_id_example' # str | 
    body = None # object | 

    try:
        # Update User Permissions
        api_response = api_instance.update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch(user_id, body)
        print("The response of RolesApi->update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **str**|  | 
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

# **update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch_0**
> object update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch_0(user_id, body)

Update User Permissions

Update individual permissions for a user (custom override).

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
    api_instance = sensecore.RolesApi(api_client)
    user_id = 'user_id_example' # str | 
    body = None # object | 

    try:
        # Update User Permissions
        api_response = api_instance.update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch_0(user_id, body)
        print("The response of RolesApi->update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch_0:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RolesApi->update_user_permissions_api_v1_admin_roles_users_user_id_permissions_patch_0: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **str**|  | 
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

