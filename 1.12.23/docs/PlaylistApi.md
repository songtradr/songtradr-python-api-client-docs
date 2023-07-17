# songtradr_api_client_python.PlaylistApi

All URIs are relative to *https://api.songtradr.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**all_playlists**](PlaylistApi.md#all_playlists) | **GET** /api/v1/playlist | All playlists.
[**create_or_update_playlist**](PlaylistApi.md#create_or_update_playlist) | **POST** /api/v1/playlist | Create and edit playlist.
[**delete_playlist**](PlaylistApi.md#delete_playlist) | **DELETE** /api/v1/playlist/{songtradrPlaylistGuid} | Delete playlist.


# **all_playlists**
> List[PlaylistLargeDTO] all_playlists(include_recordings=include_recordings, ignore_usages=ignore_usages, usage_filter_mode=usage_filter_mode, songtradr_playlist_guid=songtradr_playlist_guid)

All playlists.

### Example

* Bearer (JWT) Authentication (bearer-jwt):
```python
import time
import os
import songtradr_api_client_python
from songtradr_api_client_python.models.playlist_large_dto import PlaylistLargeDTO
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
    api_instance = songtradr_api_client_python.PlaylistApi(api_client)
    include_recordings = False # bool | Whether a playlist shall include recordings or not. (optional) (default to False)
    ignore_usages = False # bool | Whether a playlist shall include all songs regardless of their track usages. (optional) (default to False)
    usage_filter_mode = 'any' # str | Whether a playlist recordings shall include all playlist usages or not. (optional) (default to 'any')
    songtradr_playlist_guid = 'songtradr_playlist_guid_example' # str |  (optional)

    try:
        # All playlists.
        api_response = api_instance.all_playlists(include_recordings=include_recordings, ignore_usages=ignore_usages, usage_filter_mode=usage_filter_mode, songtradr_playlist_guid=songtradr_playlist_guid)
        print("The response of PlaylistApi->all_playlists:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PlaylistApi->all_playlists: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **include_recordings** | **bool**| Whether a playlist shall include recordings or not. | [optional] [default to False]
 **ignore_usages** | **bool**| Whether a playlist shall include all songs regardless of their track usages. | [optional] [default to False]
 **usage_filter_mode** | **str**| Whether a playlist recordings shall include all playlist usages or not. | [optional] [default to &#39;any&#39;]
 **songtradr_playlist_guid** | **str**|  | [optional] 

### Return type

[**List[PlaylistLargeDTO]**](PlaylistLargeDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Found playlists. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **create_or_update_playlist**
> object create_or_update_playlist(save_playlist_dto)

Create and edit playlist.

This endpoint expects always the full amount of information including all recordings.

### Example

* Bearer (JWT) Authentication (bearer-jwt):
```python
import time
import os
import songtradr_api_client_python
from songtradr_api_client_python.models.save_playlist_dto import SavePlaylistDTO
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
    api_instance = songtradr_api_client_python.PlaylistApi(api_client)
    save_playlist_dto = songtradr_api_client_python.SavePlaylistDTO() # SavePlaylistDTO | 

    try:
        # Create and edit playlist.
        api_response = api_instance.create_or_update_playlist(save_playlist_dto)
        print("The response of PlaylistApi->create_or_update_playlist:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PlaylistApi->create_or_update_playlist: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **save_playlist_dto** | [**SavePlaylistDTO**](SavePlaylistDTO.md)|  | 

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
**403** | Not allowed to edit playlist. |  -  |
**200** | Edited metadata of playlist. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_playlist**
> object delete_playlist(songtradr_playlist_guid)

Delete playlist.

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
    api_instance = songtradr_api_client_python.PlaylistApi(api_client)
    songtradr_playlist_guid = '1234' # str | ID of the file that should be deleted.

    try:
        # Delete playlist.
        api_response = api_instance.delete_playlist(songtradr_playlist_guid)
        print("The response of PlaylistApi->delete_playlist:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PlaylistApi->delete_playlist: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **songtradr_playlist_guid** | **str**| ID of the file that should be deleted. | 

### Return type

**object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/hal+json, application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Deleted playlist. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

