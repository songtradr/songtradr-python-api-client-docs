# songtradr_api_client_python.AllowedValuesApi

All URIs are relative to *https://api.songtradr.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allowed_musical_features**](AllowedValuesApi.md#allowed_musical_features) | **GET** /api/v1/allowedValues/musicalFeatures | Allowed values for music descriptive parameters to be used in the searchAll endpoint.


# **allowed_musical_features**
> SearchFilterValuesDTO allowed_musical_features(response_size=response_size)

Allowed values for music descriptive parameters to be used in the searchAll endpoint.

### Example


```python
import songtradr_api_client_python
from songtradr_api_client_python.models.search_filter_values_dto import SearchFilterValuesDTO
from songtradr_api_client_python.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to https://api.songtradr.com
# See configuration.py for a list of all supported configuration parameters.
configuration = songtradr_api_client_python.Configuration(
    host = "https://api.songtradr.com"
)


# Enter a context with an instance of the API client
with songtradr_api_client_python.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = songtradr_api_client_python.AllowedValuesApi(api_client)
    response_size = 's' # str | Size the response should have. (optional) (default to 's')

    try:
        # Allowed values for music descriptive parameters to be used in the searchAll endpoint.
        api_response = api_instance.allowed_musical_features(response_size=response_size)
        print("The response of AllowedValuesApi->allowed_musical_features:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AllowedValuesApi->allowed_musical_features: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **response_size** | **str**| Size the response should have. | [optional] [default to &#39;s&#39;]

### Return type

[**SearchFilterValuesDTO**](SearchFilterValuesDTO.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Retrieved searchFilters |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

