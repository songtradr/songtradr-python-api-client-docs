# songtradr_api_client_python.InternalApiApi

All URIs are relative to *https://api.songtradr.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**internal_create_inference**](InternalApiApi.md#internal_create_inference) | **POST** /api/v1/internal/inference | 
[**internal_update_file**](InternalApiApi.md#internal_update_file) | **PATCH** /api/v1/internal/file/{customerName}/{objectKey} | 


# **internal_create_inference**
> object internal_create_inference(authorization, save_file_recording_dto)



### Example

* Bearer (JWT) Authentication (bearer-jwt):
```python
import time
import os
import songtradr_api_client_python
from songtradr_api_client_python.models.save_file_recording_dto import SaveFileRecordingDTO
from songtradr_api_client_python.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.songtradr.com
# See configuration.py for a list of all supported configuration parameters.
configuration = songtradr_api_client_python.Configuration(
    host = "https://api.songtradr.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearer-jwt
configuration = songtradr_api_client_python.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with songtradr_api_client_python.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = songtradr_api_client_python.InternalApiApi(api_client)
    authorization = 'authorization_example' # str | 
    save_file_recording_dto = [songtradr_api_client_python.SaveFileRecordingDTO()] # List[SaveFileRecordingDTO] | 

    try:
        api_response = api_instance.internal_create_inference(authorization, save_file_recording_dto)
        print("The response of InternalApiApi->internal_create_inference:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InternalApiApi->internal_create_inference: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **str**|  | 
 **save_file_recording_dto** | [**List[SaveFileRecordingDTO]**](SaveFileRecordingDTO.md)|  | 

### Return type

**object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **internal_update_file**
> object internal_update_file(customer_name, object_key, save_file_dto)



### Example

* Bearer (JWT) Authentication (bearer-jwt):
```python
import time
import os
import songtradr_api_client_python
from songtradr_api_client_python.models.save_file_dto import SaveFileDTO
from songtradr_api_client_python.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.songtradr.com
# See configuration.py for a list of all supported configuration parameters.
configuration = songtradr_api_client_python.Configuration(
    host = "https://api.songtradr.com"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization (JWT): bearer-jwt
configuration = songtradr_api_client_python.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with songtradr_api_client_python.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = songtradr_api_client_python.InternalApiApi(api_client)
    customer_name = 'customer_name_example' # str | 
    object_key = 'object_key_example' # str | 
    save_file_dto = songtradr_api_client_python.SaveFileDTO() # SaveFileDTO | 

    try:
        api_response = api_instance.internal_update_file(customer_name, object_key, save_file_dto)
        print("The response of InternalApiApi->internal_update_file:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling InternalApiApi->internal_update_file: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customer_name** | **str**|  | 
 **object_key** | **str**|  | 
 **save_file_dto** | [**SaveFileDTO**](SaveFileDTO.md)|  | 

### Return type

**object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | OK |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

