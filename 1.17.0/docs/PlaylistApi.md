# songtradr_api_client_python.PlaylistApi

All URIs are relative to *https://api.songtradr.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**curate_playlist**](PlaylistApi.md#curate_playlist) | **POST** /api/v1/playlist/{methodName} | Curate playlist.


# **curate_playlist**
> CuratePlaylistResponseDTO curate_playlist(method_name, curate_playlist_dto)

Curate playlist.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.curate_playlist_dto import CuratePlaylistDTO
from songtradr_api_client_python.models.curate_playlist_response_dto import CuratePlaylistResponseDTO
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
    method_name = 'method_name_example' # str | Name of the curation task that should be executed
    curate_playlist_dto = songtradr_api_client_python.CuratePlaylistDTO() # CuratePlaylistDTO | 

    try:
        # Curate playlist.
        api_response = api_instance.curate_playlist(method_name, curate_playlist_dto)
        print("The response of PlaylistApi->curate_playlist:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling PlaylistApi->curate_playlist: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **method_name** | **str**| Name of the curation task that should be executed | 
 **curate_playlist_dto** | [**CuratePlaylistDTO**](CuratePlaylistDTO.md)|  | 

### Return type

[**CuratePlaylistResponseDTO**](CuratePlaylistResponseDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**403** | Not allowed to edit playlist. |  -  |
**200** | Playlist curated. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

