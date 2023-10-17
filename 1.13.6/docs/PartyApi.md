# songtradr_api_client_python.PartyApi

All URIs are relative to *https://api.songtradr.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**party**](PartyApi.md#party) | **GET** /api/v1/party | Information on a person, group or company.


# **party**
> PartyLargeDTO party(full_name)

Information on a person, group or company.

### Example

* Bearer (JWT) Authentication (bearer-jwt):
```python
import time
import os
import songtradr_api_client_python
from songtradr_api_client_python.models.party_large_dto import PartyLargeDTO
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
    api_instance = songtradr_api_client_python.PartyApi(api_client)
    full_name = 'The Beatles' # str | Full Name of the person, group, company or organisation.

    try:
        # Information on a person, group or company.
        api_response = api_instance.party(full_name)
        print("The response of PartyApi->party:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PartyApi->party: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **full_name** | **str**| Full Name of the person, group, company or organisation. | 

### Return type

[**PartyLargeDTO**](PartyLargeDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Found artist. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

