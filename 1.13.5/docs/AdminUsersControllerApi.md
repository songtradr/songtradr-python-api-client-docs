# songtradr_api_client_python.AdminUsersControllerApi

All URIs are relative to *https://api.songtradr.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_user**](AdminUsersControllerApi.md#create_user) | **POST** /api/v1/admin/users | create a user
[**delete_user**](AdminUsersControllerApi.md#delete_user) | **DELETE** /api/v1/admin/users/{id} | delete a user
[**get_user**](AdminUsersControllerApi.md#get_user) | **GET** /api/v1/admin/users/{id} | show details of a user
[**get_users**](AdminUsersControllerApi.md#get_users) | **GET** /api/v1/admin/users | List users
[**update_user**](AdminUsersControllerApi.md#update_user) | **PUT** /api/v1/admin/users/{id} | update a user


# **create_user**
> AdminApiUserDTO create_user(admin_api_create_user_dto)

create a user

### Example

* Bearer (JWT) Authentication (bearer-jwt):
```python
import time
import os
import songtradr_api_client_python
from songtradr_api_client_python.models.admin_api_create_user_dto import AdminApiCreateUserDTO
from songtradr_api_client_python.models.admin_api_user_dto import AdminApiUserDTO
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
    api_instance = songtradr_api_client_python.AdminUsersControllerApi(api_client)
    admin_api_create_user_dto = songtradr_api_client_python.AdminApiCreateUserDTO() # AdminApiCreateUserDTO | 

    try:
        # create a user
        api_response = api_instance.create_user(admin_api_create_user_dto)
        print("The response of AdminUsersControllerApi->create_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AdminUsersControllerApi->create_user: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **admin_api_create_user_dto** | [**AdminApiCreateUserDTO**](AdminApiCreateUserDTO.md)|  | 

### Return type

[**AdminApiUserDTO**](AdminApiUserDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | return created user |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_user**
> object delete_user(id)

delete a user

### Example

* Bearer (JWT) Authentication (bearer-jwt):
```python
import time
import os
import songtradr_api_client_python
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
    api_instance = songtradr_api_client_python.AdminUsersControllerApi(api_client)
    id = 56 # int | 

    try:
        # delete a user
        api_response = api_instance.delete_user(id)
        print("The response of AdminUsersControllerApi->delete_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AdminUsersControllerApi->delete_user: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

**object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | deleted user |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_user**
> AdminApiUserDTO get_user(id)

show details of a user

### Example

* Bearer (JWT) Authentication (bearer-jwt):
```python
import time
import os
import songtradr_api_client_python
from songtradr_api_client_python.models.admin_api_user_dto import AdminApiUserDTO
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
    api_instance = songtradr_api_client_python.AdminUsersControllerApi(api_client)
    id = 56 # int | 

    try:
        # show details of a user
        api_response = api_instance.get_user(id)
        print("The response of AdminUsersControllerApi->get_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AdminUsersControllerApi->get_user: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 

### Return type

[**AdminApiUserDTO**](AdminApiUserDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | found user details. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_users**
> AdminApiUserDTO get_users(page=page, size=size, sort=sort)

List users

### Example

* Bearer (JWT) Authentication (bearer-jwt):
```python
import time
import os
import songtradr_api_client_python
from songtradr_api_client_python.models.admin_api_user_dto import AdminApiUserDTO
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
    api_instance = songtradr_api_client_python.AdminUsersControllerApi(api_client)
    page = 0 # int | Zero-based page index (0..N) (optional) (default to 0)
    size = 20 # int | The size of the page to be returned (optional) (default to 20)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        # List users
        api_response = api_instance.get_users(page=page, size=size, sort=sort)
        print("The response of AdminUsersControllerApi->get_users:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AdminUsersControllerApi->get_users: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**| Zero-based page index (0..N) | [optional] [default to 0]
 **size** | **int**| The size of the page to be returned | [optional] [default to 20]
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 

### Return type

[**AdminApiUserDTO**](AdminApiUserDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | found users |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_user**
> AdminApiUserDTO update_user(id, admin_api_update_user_dto)

update a user

### Example

* Bearer (JWT) Authentication (bearer-jwt):
```python
import time
import os
import songtradr_api_client_python
from songtradr_api_client_python.models.admin_api_update_user_dto import AdminApiUpdateUserDTO
from songtradr_api_client_python.models.admin_api_user_dto import AdminApiUserDTO
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
    api_instance = songtradr_api_client_python.AdminUsersControllerApi(api_client)
    id = 56 # int | 
    admin_api_update_user_dto = songtradr_api_client_python.AdminApiUpdateUserDTO() # AdminApiUpdateUserDTO | 

    try:
        # update a user
        api_response = api_instance.update_user(id, admin_api_update_user_dto)
        print("The response of AdminUsersControllerApi->update_user:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AdminUsersControllerApi->update_user: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  | 
 **admin_api_update_user_dto** | [**AdminApiUpdateUserDTO**](AdminApiUpdateUserDTO.md)|  | 

### Return type

[**AdminApiUserDTO**](AdminApiUserDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | found user details. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

