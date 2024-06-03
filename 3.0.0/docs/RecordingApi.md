# songtradr_api_client_python.RecordingApi

All URIs are relative to *https://api.songtradr.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**recordings_by_ids_with_taggrams1**](RecordingApi.md#recordings_by_ids_with_taggrams1) | **GET** /api/v1/public/recording/{ids}/taggrams | Timeseries of AI generated moods, musical features and more for a list of recordings.
[**recordings_by_ids_with_tagstrengths1**](RecordingApi.md#recordings_by_ids_with_tagstrengths1) | **GET** /api/v1/public/recording/{ids}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings.
[**recordings_medium_by_ids1**](RecordingApi.md#recordings_medium_by_ids1) | **GET** /api/v1/public/recording/m/{ids} | Recordings by IDs with a medium sized response.


# **recordings_by_ids_with_taggrams1**
> List[RecordingMinimalWithTaggramsDTO] recordings_by_ids_with_taggrams1(ids, category_name=category_name, tag_name=tag_name, genre_name=genre_name, from_timestamp=from_timestamp, to_timestamp=to_timestamp, fill_with_zero=fill_with_zero)

Timeseries of AI generated moods, musical features and more for a list of recordings.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.recording_minimal_with_taggrams_dto import RecordingMinimalWithTaggramsDTO
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
    api_instance = songtradr_api_client_python.RecordingApi(api_client)
    ids = 'USUM71703692' # str | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
    category_name = 'moodCluster' # str | Show only taggrams for one category. (optional)
    tag_name = 'energetic' # str | Show only taggrams for one tag. (optional)
    genre_name = 'Ska' # str | Show only taggrams for one genre. (optional)
    from_timestamp = 16.0 # float | Show only taggrams data starting from from this timestamp in seconds. (optional)
    to_timestamp = 32.0 # float | Show only taggrams data before this timestamp in seconds. (optional)
    fill_with_zero = true # bool | If set to true, empty timeseries are filled with timeseries of 0.0 values. (optional)

    try:
        # Timeseries of AI generated moods, musical features and more for a list of recordings.
        api_response = api_instance.recordings_by_ids_with_taggrams1(ids, category_name=category_name, tag_name=tag_name, genre_name=genre_name, from_timestamp=from_timestamp, to_timestamp=to_timestamp, fill_with_zero=fill_with_zero)
        print("The response of RecordingApi->recordings_by_ids_with_taggrams1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordingApi->recordings_by_ids_with_taggrams1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ids** | **str**| Comma seperated list of IDs. Can be ISRCs or proprietary IDs | 
 **category_name** | **str**| Show only taggrams for one category. | [optional] 
 **tag_name** | **str**| Show only taggrams for one tag. | [optional] 
 **genre_name** | **str**| Show only taggrams for one genre. | [optional] 
 **from_timestamp** | **float**| Show only taggrams data starting from from this timestamp in seconds. | [optional] 
 **to_timestamp** | **float**| Show only taggrams data before this timestamp in seconds. | [optional] 
 **fill_with_zero** | **bool**| If set to true, empty timeseries are filled with timeseries of 0.0 values. | [optional] 

### Return type

[**List[RecordingMinimalWithTaggramsDTO]**](RecordingMinimalWithTaggramsDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Found recordings. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **recordings_by_ids_with_tagstrengths1**
> List[RecordingMinimalWithTagstrengthsDTO] recordings_by_ids_with_tagstrengths1(ids, category_name=category_name, tag_name=tag_name, genre_name=genre_name)

Strengths as numerical representations for AI generated moods, musical features and more for recordings.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.recording_minimal_with_tagstrengths_dto import RecordingMinimalWithTagstrengthsDTO
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
    api_instance = songtradr_api_client_python.RecordingApi(api_client)
    ids = 'USUM71703692' # str | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
    category_name = 'moodCluster' # str | Show only taggrams for one category. (optional)
    tag_name = 'energetic' # str | Show only taggrams for one tag. (optional)
    genre_name = 'Ska' # str | Show only taggrams for one genre. (optional)

    try:
        # Strengths as numerical representations for AI generated moods, musical features and more for recordings.
        api_response = api_instance.recordings_by_ids_with_tagstrengths1(ids, category_name=category_name, tag_name=tag_name, genre_name=genre_name)
        print("The response of RecordingApi->recordings_by_ids_with_tagstrengths1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordingApi->recordings_by_ids_with_tagstrengths1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ids** | **str**| Comma seperated list of IDs. Can be ISRCs or proprietary IDs | 
 **category_name** | **str**| Show only taggrams for one category. | [optional] 
 **tag_name** | **str**| Show only taggrams for one tag. | [optional] 
 **genre_name** | **str**| Show only taggrams for one genre. | [optional] 

### Return type

[**List[RecordingMinimalWithTagstrengthsDTO]**](RecordingMinimalWithTagstrengthsDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Found recordings. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **recordings_medium_by_ids1**
> List[RecordingMediumDTO] recordings_medium_by_ids1(ids, page=page, size=size, sort=sort)

Recordings by IDs with a medium sized response.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.recording_medium_dto import RecordingMediumDTO
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
    api_instance = songtradr_api_client_python.RecordingApi(api_client)
    ids = 'GBAHT0108619' # str | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
    page = 0 # int | Zero-based page index (0..N) (optional) (default to 0)
    size = 20 # int | The size of the page to be returned (optional) (default to 20)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        # Recordings by IDs with a medium sized response.
        api_response = api_instance.recordings_medium_by_ids1(ids, page=page, size=size, sort=sort)
        print("The response of RecordingApi->recordings_medium_by_ids1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordingApi->recordings_medium_by_ids1: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ids** | **str**| Comma seperated list of IDs. Can be ISRCs or proprietary IDs | 
 **page** | **int**| Zero-based page index (0..N) | [optional] [default to 0]
 **size** | **int**| The size of the page to be returned | [optional] [default to 20]
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 

### Return type

[**List[RecordingMediumDTO]**](RecordingMediumDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Found recordings. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

