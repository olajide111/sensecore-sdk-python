# sensecore.AuthApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_me_api_v1_auth_me_get**](AuthApi.md#get_me_api_v1_auth_me_get) | **GET** /api/v1/auth/me | Get Me
[**login_api_v1_auth_login_post**](AuthApi.md#login_api_v1_auth_login_post) | **POST** /api/v1/auth/login | Get access token
[**my_permissions_api_v1_me_permissions_get**](AuthApi.md#my_permissions_api_v1_me_permissions_get) | **GET** /api/v1/me/permissions | My Permissions
[**register_api_v1_auth_register_post**](AuthApi.md#register_api_v1_auth_register_post) | **POST** /api/v1/auth/register | Register
[**reset_password_api_v1_auth_reset_password_post**](AuthApi.md#reset_password_api_v1_auth_reset_password_post) | **POST** /api/v1/auth/reset-password | Reset Password
[**verify_api_v1_auth_verify_get**](AuthApi.md#verify_api_v1_auth_verify_get) | **GET** /api/v1/auth/verify | Verify


# **get_me_api_v1_auth_me_get**
> object get_me_api_v1_auth_me_get()

Get Me

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
    api_instance = sensecore.AuthApi(api_client)

    try:
        # Get Me
        api_response = api_instance.get_me_api_v1_auth_me_get()
        print("The response of AuthApi->get_me_api_v1_auth_me_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->get_me_api_v1_auth_me_get: %s\n" % e)
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

# **login_api_v1_auth_login_post**
> object login_api_v1_auth_login_post(username, password, grant_type=grant_type, scope=scope, client_id=client_id, client_secret=client_secret)

Get access token

Exchange email + password for a JWT access token.
Include token in all requests: `Authorization: Bearer <token>`

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
    api_instance = sensecore.AuthApi(api_client)
    username = 'username_example' # str | 
    password = 'password_example' # str | 
    grant_type = 'grant_type_example' # str |  (optional)
    scope = '' # str |  (optional) (default to '')
    client_id = 'client_id_example' # str |  (optional)
    client_secret = 'client_secret_example' # str |  (optional)

    try:
        # Get access token
        api_response = api_instance.login_api_v1_auth_login_post(username, password, grant_type=grant_type, scope=scope, client_id=client_id, client_secret=client_secret)
        print("The response of AuthApi->login_api_v1_auth_login_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->login_api_v1_auth_login_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **username** | **str**|  | 
 **password** | **str**|  | 
 **grant_type** | **str**|  | [optional] 
 **scope** | **str**|  | [optional] [default to &#39;&#39;]
 **client_id** | **str**|  | [optional] 
 **client_secret** | **str**|  | [optional] 

### Return type

**object**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **my_permissions_api_v1_me_permissions_get**
> object my_permissions_api_v1_me_permissions_get()

My Permissions

Return current user role and permissions for frontend gating.

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
    api_instance = sensecore.AuthApi(api_client)

    try:
        # My Permissions
        api_response = api_instance.my_permissions_api_v1_me_permissions_get()
        print("The response of AuthApi->my_permissions_api_v1_me_permissions_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->my_permissions_api_v1_me_permissions_get: %s\n" % e)
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

# **register_api_v1_auth_register_post**
> Dict[str, Optional[str]] register_api_v1_auth_register_post(register_request)

Register

### Example


```python
import sensecore
from sensecore.models.register_request import RegisterRequest
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
    api_instance = sensecore.AuthApi(api_client)
    register_request = sensecore.RegisterRequest() # RegisterRequest | 

    try:
        # Register
        api_response = api_instance.register_api_v1_auth_register_post(register_request)
        print("The response of AuthApi->register_api_v1_auth_register_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->register_api_v1_auth_register_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **register_request** | [**RegisterRequest**](RegisterRequest.md)|  | 

### Return type

**Dict[str, Optional[str]]**

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

# **reset_password_api_v1_auth_reset_password_post**
> Dict[str, Optional[str]] reset_password_api_v1_auth_reset_password_post(reset_request)

Reset Password

### Example


```python
import sensecore
from sensecore.models.reset_request import ResetRequest
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
    api_instance = sensecore.AuthApi(api_client)
    reset_request = sensecore.ResetRequest() # ResetRequest | 

    try:
        # Reset Password
        api_response = api_instance.reset_password_api_v1_auth_reset_password_post(reset_request)
        print("The response of AuthApi->reset_password_api_v1_auth_reset_password_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->reset_password_api_v1_auth_reset_password_post: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **reset_request** | [**ResetRequest**](ResetRequest.md)|  | 

### Return type

**Dict[str, Optional[str]]**

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

# **verify_api_v1_auth_verify_get**
> Dict[str, Optional[str]] verify_api_v1_auth_verify_get(token)

Verify

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
    api_instance = sensecore.AuthApi(api_client)
    token = 'token_example' # str | Email verification token

    try:
        # Verify
        api_response = api_instance.verify_api_v1_auth_verify_get(token)
        print("The response of AuthApi->verify_api_v1_auth_verify_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AuthApi->verify_api_v1_auth_verify_get: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token** | **str**| Email verification token | 

### Return type

**Dict[str, Optional[str]]**

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

