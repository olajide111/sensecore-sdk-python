# sensecore.MLOpsApi

All URIs are relative to *https://api.sensecoreai.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_training_job_api_v1_admin_mlops_training_jobs_post**](MLOpsApi.md#create_training_job_api_v1_admin_mlops_training_jobs_post) | **POST** /api/v1/admin/mlops/training-jobs | Create Training Job
[**get_model_performance_api_v1_admin_mlops_performance_get**](MLOpsApi.md#get_model_performance_api_v1_admin_mlops_performance_get) | **GET** /api/v1/admin/mlops/performance | Get Model Performance
[**list_checkpoints_detailed_api_v1_admin_mlops_checkpoints_get**](MLOpsApi.md#list_checkpoints_detailed_api_v1_admin_mlops_checkpoints_get) | **GET** /api/v1/admin/mlops/checkpoints | List Checkpoints Detailed
[**list_training_jobs_api_v1_admin_mlops_training_jobs_get**](MLOpsApi.md#list_training_jobs_api_v1_admin_mlops_training_jobs_get) | **GET** /api/v1/admin/mlops/training-jobs | List Training Jobs
[**set_retrain_schedule_api_v1_admin_mlops_schedule_post**](MLOpsApi.md#set_retrain_schedule_api_v1_admin_mlops_schedule_post) | **POST** /api/v1/admin/mlops/schedule | Set Retrain Schedule
[**update_training_job_api_v1_admin_mlops_training_jobs_job_id_patch**](MLOpsApi.md#update_training_job_api_v1_admin_mlops_training_jobs_job_id_patch) | **PATCH** /api/v1/admin/mlops/training-jobs/{job_id} | Update Training Job


# **create_training_job_api_v1_admin_mlops_training_jobs_post**
> object create_training_job_api_v1_admin_mlops_training_jobs_post(body)

Create Training Job

3D.2 — Queue a new training job

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
    api_instance = sensecore.MLOpsApi(api_client)
    body = None # object | 

    try:
        # Create Training Job
        api_response = api_instance.create_training_job_api_v1_admin_mlops_training_jobs_post(body)
        print("The response of MLOpsApi->create_training_job_api_v1_admin_mlops_training_jobs_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MLOpsApi->create_training_job_api_v1_admin_mlops_training_jobs_post: %s\n" % e)
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

# **get_model_performance_api_v1_admin_mlops_performance_get**
> object get_model_performance_api_v1_admin_mlops_performance_get()

Get Model Performance

3D.3 — MAPE tracking over time

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
    api_instance = sensecore.MLOpsApi(api_client)

    try:
        # Get Model Performance
        api_response = api_instance.get_model_performance_api_v1_admin_mlops_performance_get()
        print("The response of MLOpsApi->get_model_performance_api_v1_admin_mlops_performance_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MLOpsApi->get_model_performance_api_v1_admin_mlops_performance_get: %s\n" % e)
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

# **list_checkpoints_detailed_api_v1_admin_mlops_checkpoints_get**
> object list_checkpoints_detailed_api_v1_admin_mlops_checkpoints_get()

List Checkpoints Detailed

3D.6 — Model checkpoint details with S3 backup status

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
    api_instance = sensecore.MLOpsApi(api_client)

    try:
        # List Checkpoints Detailed
        api_response = api_instance.list_checkpoints_detailed_api_v1_admin_mlops_checkpoints_get()
        print("The response of MLOpsApi->list_checkpoints_detailed_api_v1_admin_mlops_checkpoints_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MLOpsApi->list_checkpoints_detailed_api_v1_admin_mlops_checkpoints_get: %s\n" % e)
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

# **list_training_jobs_api_v1_admin_mlops_training_jobs_get**
> object list_training_jobs_api_v1_admin_mlops_training_jobs_get()

List Training Jobs

3D.2 — List training jobs (start, monitor, cancel)

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
    api_instance = sensecore.MLOpsApi(api_client)

    try:
        # List Training Jobs
        api_response = api_instance.list_training_jobs_api_v1_admin_mlops_training_jobs_get()
        print("The response of MLOpsApi->list_training_jobs_api_v1_admin_mlops_training_jobs_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MLOpsApi->list_training_jobs_api_v1_admin_mlops_training_jobs_get: %s\n" % e)
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

# **set_retrain_schedule_api_v1_admin_mlops_schedule_post**
> object set_retrain_schedule_api_v1_admin_mlops_schedule_post(body)

Set Retrain Schedule

3D.5 — Set retrain schedule (auto or manual)

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
    api_instance = sensecore.MLOpsApi(api_client)
    body = None # object | 

    try:
        # Set Retrain Schedule
        api_response = api_instance.set_retrain_schedule_api_v1_admin_mlops_schedule_post(body)
        print("The response of MLOpsApi->set_retrain_schedule_api_v1_admin_mlops_schedule_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MLOpsApi->set_retrain_schedule_api_v1_admin_mlops_schedule_post: %s\n" % e)
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

# **update_training_job_api_v1_admin_mlops_training_jobs_job_id_patch**
> object update_training_job_api_v1_admin_mlops_training_jobs_job_id_patch(job_id, body)

Update Training Job

3D.2 — Update job status (called by training script)

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
    api_instance = sensecore.MLOpsApi(api_client)
    job_id = 'job_id_example' # str | 
    body = None # object | 

    try:
        # Update Training Job
        api_response = api_instance.update_training_job_api_v1_admin_mlops_training_jobs_job_id_patch(job_id, body)
        print("The response of MLOpsApi->update_training_job_api_v1_admin_mlops_training_jobs_job_id_patch:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling MLOpsApi->update_training_job_api_v1_admin_mlops_training_jobs_job_id_patch: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **job_id** | **str**|  | 
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

