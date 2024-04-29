# songtradr_api_client_python.UserApi

All URIs are relative to *https://api.songtradr.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**delete_user_file**](UserApi.md#delete_user_file) | **DELETE** /api/v1/user/file/{objectKey} | Delete file.
[**edit_me**](UserApi.md#edit_me) | **POST** /api/v1/user/me | Edit details for a logged-in user
[**forgot_password**](UserApi.md#forgot_password) | **POST** /api/v1/user/forgot-password | Send a password reset email
[**init_video_upload**](UserApi.md#init_video_upload) | **POST** /api/v1/user/file/{name}/initVideoUpload | Recognise and upload video. Responds with an object with recognition result.
[**initiate_user_file_upload**](UserApi.md#initiate_user_file_upload) | **POST** /api/v1/user/file/{name}/initUpload | Initialize a file upload. Responds with an URL where the file can be uploaded.
[**initiate_user_image_upload**](UserApi.md#initiate_user_image_upload) | **POST** /api/v1/user/file/{name}/initImageUpload | Recognise and upload image. Responds with an object with recognition result.
[**login**](UserApi.md#login) | **POST** /api/v1/user/login | Login to generate a bearer token.
[**me**](UserApi.md#me) | **GET** /api/v1/user/me | Details for a logged-in user
[**prompt_search_user_files**](UserApi.md#prompt_search_user_files) | **GET** /api/v1/user/promptSearch | Files for query.
[**recordings_by_folder_with_taggrams**](UserApi.md#recordings_by_folder_with_taggrams) | **GET** /api/v1/user/folder/{folderName}/taggrams | Timeseries of AI generated moods, musical features and more for recordings in your folder.
[**recordings_by_folder_with_tagstrengths**](UserApi.md#recordings_by_folder_with_tagstrengths) | **GET** /api/v1/user/folder/{folderName}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.
[**recordings_by_ids_with_similarities**](UserApi.md#recordings_by_ids_with_similarities) | **GET** /api/v1/user/recording/{ids}/similarities | Similar recordings for a list of user recordings.
[**recordings_by_ids_with_taggrams**](UserApi.md#recordings_by_ids_with_taggrams) | **GET** /api/v1/user/recording/{ids}/taggrams | Timeseries of AI generated moods, musical features and more for a list of recordings.
[**recordings_by_ids_with_tagstrengths**](UserApi.md#recordings_by_ids_with_tagstrengths) | **GET** /api/v1/user/recording/{ids}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings.
[**recordings_medium_by_ids**](UserApi.md#recordings_medium_by_ids) | **GET** /api/v1/user/recording/{ids} | Recordings by IDs with a medium sized response.
[**sign_up**](UserApi.md#sign_up) | **POST** /api/v1/user/sign-up | Sign up a new user.
[**token**](UserApi.md#token) | **POST** /api/v1/user/token | Generates a new JWT token for the given refresh token
[**update_password**](UserApi.md#update_password) | **POST** /api/v1/user/update-password | Update password by using the password reset token
[**user_file**](UserApi.md#user_file) | **GET** /api/v1/user/file/{objectKey} | Details and a download link for a file.
[**user_files**](UserApi.md#user_files) | **GET** /api/v1/user/files | List and search your own files.
[**user_files_status**](UserApi.md#user_files_status) | **GET** /api/v1/user/filesStatus | Status details for files.
[**user_files_summary**](UserApi.md#user_files_summary) | **GET** /api/v1/user/filesSummary | Summary fo your files.


# **delete_user_file**
> object delete_user_file(object_key)

Delete file.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    object_key = '73818371-0963-412e-aa3d-27c2bab952a3' # str | ObjectKey of the file that should be deleted.

    try:
        # Delete file.
        api_response = api_instance.delete_user_file(object_key)
        print("The response of UserApi->delete_user_file:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->delete_user_file: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_key** | **str**| ObjectKey of the file that should be deleted. | 

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
**200** | Deleted file. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **edit_me**
> object edit_me(save_user_dto)

Edit details for a logged-in user

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.save_user_dto import SaveUserDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    save_user_dto = songtradr_api_client_python.SaveUserDTO() # SaveUserDTO | 

    try:
        # Edit details for a logged-in user
        api_response = api_instance.edit_me(save_user_dto)
        print("The response of UserApi->edit_me:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->edit_me: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **save_user_dto** | [**SaveUserDTO**](SaveUserDTO.md)|  | 

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
**200** | Edited user details. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **forgot_password**
> object forgot_password(forgot_password_dto)

Send a password reset email

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.forgot_password_dto import ForgotPasswordDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    forgot_password_dto = songtradr_api_client_python.ForgotPasswordDTO() # ForgotPasswordDTO | 

    try:
        # Send a password reset email
        api_response = api_instance.forgot_password(forgot_password_dto)
        print("The response of UserApi->forgot_password:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->forgot_password: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **forgot_password_dto** | [**ForgotPasswordDTO**](ForgotPasswordDTO.md)|  | 

### Return type

**object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/hal+json, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Password reset email was sent if user exist. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **init_video_upload**
> VideoRecognitionResponse init_video_upload(name, url)

Recognise and upload video. Responds with an object with recognition result.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.video_recognition_response import VideoRecognitionResponse
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    name = 'FileName.mp4' # str | The Name of the image that will be uploaded
    url = 'url_example' # str | 

    try:
        # Recognise and upload video. Responds with an object with recognition result.
        api_response = api_instance.init_video_upload(name, url)
        print("The response of UserApi->init_video_upload:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->init_video_upload: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| The Name of the image that will be uploaded | 
 **url** | **str**|  | 

### Return type

[**VideoRecognitionResponse**](VideoRecognitionResponse.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Video recognised. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **initiate_user_file_upload**
> InitPutRecordingAudioDTO initiate_user_file_upload(name, folder, file_upload_dto=file_upload_dto)

Initialize a file upload. Responds with an URL where the file can be uploaded.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.file_upload_dto import FileUploadDTO
from songtradr_api_client_python.models.init_put_recording_audio_dto import InitPutRecordingAudioDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    name = 'FileName.mp3' # str | The Name of the file that will be uploaded
    folder = 'FolderName' # str | The Name of the folder that the file will be placed in
    file_upload_dto = songtradr_api_client_python.FileUploadDTO() # FileUploadDTO |  (optional)

    try:
        # Initialize a file upload. Responds with an URL where the file can be uploaded.
        api_response = api_instance.initiate_user_file_upload(name, folder, file_upload_dto=file_upload_dto)
        print("The response of UserApi->initiate_user_file_upload:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->initiate_user_file_upload: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| The Name of the file that will be uploaded | 
 **folder** | **str**| The Name of the folder that the file will be placed in | 
 **file_upload_dto** | [**FileUploadDTO**](FileUploadDTO.md)|  | [optional] 

### Return type

[**InitPutRecordingAudioDTO**](InitPutRecordingAudioDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Provided URL to upload file. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **initiate_user_image_upload**
> ImageRecognitionResponse initiate_user_image_upload(name, url)

Recognise and upload image. Responds with an object with recognition result.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.image_recognition_response import ImageRecognitionResponse
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    name = 'FileName.mp3' # str | The Name of the image that will be uploaded
    url = 'url_example' # str | 

    try:
        # Recognise and upload image. Responds with an object with recognition result.
        api_response = api_instance.initiate_user_image_upload(name, url)
        print("The response of UserApi->initiate_user_image_upload:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->initiate_user_image_upload: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**| The Name of the image that will be uploaded | 
 **url** | **str**|  | 

### Return type

[**ImageRecognitionResponse**](ImageRecognitionResponse.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Image recognised. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **login**
> JwtTokenDTO login(login_dto)

Login to generate a bearer token.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.jwt_token_dto import JwtTokenDTO
from songtradr_api_client_python.models.login_dto import LoginDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    login_dto = songtradr_api_client_python.LoginDTO() # LoginDTO | 

    try:
        # Login to generate a bearer token.
        api_response = api_instance.login(login_dto)
        print("The response of UserApi->login:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->login: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **login_dto** | [**LoginDTO**](LoginDTO.md)|  | 

### Return type

[**JwtTokenDTO**](JwtTokenDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Generated a bearer JWT token |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **me**
> UserDTO me()

Details for a logged-in user

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.user_dto import UserDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)

    try:
        # Details for a logged-in user
        api_response = api_instance.me()
        print("The response of UserApi->me:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->me: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**UserDTO**](UserDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Found user details. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **prompt_search_user_files**
> FileListDTO prompt_search_user_files(query)

Files for query.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.file_list_dto import FileListDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    query = 'funk, guitar, drums' # str | Query.

    try:
        # Files for query.
        api_response = api_instance.prompt_search_user_files(query)
        print("The response of UserApi->prompt_search_user_files:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->prompt_search_user_files: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **str**| Query. | 

### Return type

[**FileListDTO**](FileListDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Found files. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **recordings_by_folder_with_taggrams**
> List[RecordingMinimalWithTaggramsDTO] recordings_by_folder_with_taggrams(folder_name, category_name=category_name, tag_name=tag_name, genre_name=genre_name, from_timestamp=from_timestamp, to_timestamp=to_timestamp, fill_with_zero=fill_with_zero, page=page, size=size, sort=sort)

Timeseries of AI generated moods, musical features and more for recordings in your folder.

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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    folder_name = 'Default' # str | Folder name
    category_name = 'moodCluster' # str | Show only taggrams for one category. (optional)
    tag_name = 'energetic' # str | Show only taggrams for one tag. (optional)
    genre_name = 'Ska' # str | Show only taggrams for one genre. (optional)
    from_timestamp = 16.0 # float | Show only taggrams data starting from from this timestamp in seconds. (optional)
    to_timestamp = 32.0 # float | Show only taggrams data before this timestamp in seconds. (optional)
    fill_with_zero = true # bool | If set to true, empty timeseries are filled with timeseries of 0.0 values. (optional)
    page = 0 # int | Zero-based page index (0..N) (optional) (default to 0)
    size = 20 # int | The size of the page to be returned (optional) (default to 20)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        # Timeseries of AI generated moods, musical features and more for recordings in your folder.
        api_response = api_instance.recordings_by_folder_with_taggrams(folder_name, category_name=category_name, tag_name=tag_name, genre_name=genre_name, from_timestamp=from_timestamp, to_timestamp=to_timestamp, fill_with_zero=fill_with_zero, page=page, size=size, sort=sort)
        print("The response of UserApi->recordings_by_folder_with_taggrams:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->recordings_by_folder_with_taggrams: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **folder_name** | **str**| Folder name | 
 **category_name** | **str**| Show only taggrams for one category. | [optional] 
 **tag_name** | **str**| Show only taggrams for one tag. | [optional] 
 **genre_name** | **str**| Show only taggrams for one genre. | [optional] 
 **from_timestamp** | **float**| Show only taggrams data starting from from this timestamp in seconds. | [optional] 
 **to_timestamp** | **float**| Show only taggrams data before this timestamp in seconds. | [optional] 
 **fill_with_zero** | **bool**| If set to true, empty timeseries are filled with timeseries of 0.0 values. | [optional] 
 **page** | **int**| Zero-based page index (0..N) | [optional] [default to 0]
 **size** | **int**| The size of the page to be returned | [optional] [default to 20]
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 

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

# **recordings_by_folder_with_tagstrengths**
> List[RecordingMinimalWithTagstrengthsDTO] recordings_by_folder_with_tagstrengths(folder_name, category_name=category_name, tag_name=tag_name, genre_name=genre_name, page=page, size=size, sort=sort)

Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.

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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    folder_name = 'Default' # str | Folder name
    category_name = 'moodCluster' # str | Show only taggrams for one category. (optional)
    tag_name = 'energetic' # str | Show only taggrams for one tag. (optional)
    genre_name = 'Ska' # str | Show only taggrams for one genre. (optional)
    page = 0 # int | Zero-based page index (0..N) (optional) (default to 0)
    size = 20 # int | The size of the page to be returned (optional) (default to 20)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        # Strengths as numerical representations for AI generated moods, musical features and more for recordings in your folder.
        api_response = api_instance.recordings_by_folder_with_tagstrengths(folder_name, category_name=category_name, tag_name=tag_name, genre_name=genre_name, page=page, size=size, sort=sort)
        print("The response of UserApi->recordings_by_folder_with_tagstrengths:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->recordings_by_folder_with_tagstrengths: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **folder_name** | **str**| Folder name | 
 **category_name** | **str**| Show only taggrams for one category. | [optional] 
 **tag_name** | **str**| Show only taggrams for one tag. | [optional] 
 **genre_name** | **str**| Show only taggrams for one genre. | [optional] 
 **page** | **int**| Zero-based page index (0..N) | [optional] [default to 0]
 **size** | **int**| The size of the page to be returned | [optional] [default to 20]
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] 

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

# **recordings_by_ids_with_similarities**
> List[RecordingForSimilaritySearchDTO] recordings_by_ids_with_similarities(ids, identical_only=identical_only, usage=usage)

Similar recordings for a list of user recordings.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.recording_for_similarity_search_dto import RecordingForSimilaritySearchDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    ids = 'USUM71703692' # str | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
    identical_only = False # bool | Whether a result list shall include only identical recordings. (optional) (default to False)
    usage = 'usage_example' # str | Filter by recording usage. (optional)

    try:
        # Similar recordings for a list of user recordings.
        api_response = api_instance.recordings_by_ids_with_similarities(ids, identical_only=identical_only, usage=usage)
        print("The response of UserApi->recordings_by_ids_with_similarities:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->recordings_by_ids_with_similarities: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ids** | **str**| Comma seperated list of IDs. Can be ISRCs or proprietary IDs | 
 **identical_only** | **bool**| Whether a result list shall include only identical recordings. | [optional] [default to False]
 **usage** | **str**| Filter by recording usage. | [optional] 

### Return type

[**List[RecordingForSimilaritySearchDTO]**](RecordingForSimilaritySearchDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Found user recordings. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **recordings_by_ids_with_taggrams**
> List[RecordingMinimalWithTaggramsDTO] recordings_by_ids_with_taggrams(ids, category_name=category_name, tag_name=tag_name, genre_name=genre_name, from_timestamp=from_timestamp, to_timestamp=to_timestamp, fill_with_zero=fill_with_zero)

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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    ids = 'USUM71703692' # str | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
    category_name = 'moodCluster' # str | Show only taggrams for one category. (optional)
    tag_name = 'energetic' # str | Show only taggrams for one tag. (optional)
    genre_name = 'Ska' # str | Show only taggrams for one genre. (optional)
    from_timestamp = 16.0 # float | Show only taggrams data starting from from this timestamp in seconds. (optional)
    to_timestamp = 32.0 # float | Show only taggrams data before this timestamp in seconds. (optional)
    fill_with_zero = true # bool | If set to true, empty timeseries are filled with timeseries of 0.0 values. (optional)

    try:
        # Timeseries of AI generated moods, musical features and more for a list of recordings.
        api_response = api_instance.recordings_by_ids_with_taggrams(ids, category_name=category_name, tag_name=tag_name, genre_name=genre_name, from_timestamp=from_timestamp, to_timestamp=to_timestamp, fill_with_zero=fill_with_zero)
        print("The response of UserApi->recordings_by_ids_with_taggrams:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->recordings_by_ids_with_taggrams: %s\n" % e)
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

# **recordings_by_ids_with_tagstrengths**
> List[RecordingMinimalWithTagstrengthsDTO] recordings_by_ids_with_tagstrengths(ids, category_name=category_name, tag_name=tag_name, genre_name=genre_name)

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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    ids = 'USUM71703692' # str | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
    category_name = 'moodCluster' # str | Show only taggrams for one category. (optional)
    tag_name = 'energetic' # str | Show only taggrams for one tag. (optional)
    genre_name = 'Ska' # str | Show only taggrams for one genre. (optional)

    try:
        # Strengths as numerical representations for AI generated moods, musical features and more for recordings.
        api_response = api_instance.recordings_by_ids_with_tagstrengths(ids, category_name=category_name, tag_name=tag_name, genre_name=genre_name)
        print("The response of UserApi->recordings_by_ids_with_tagstrengths:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->recordings_by_ids_with_tagstrengths: %s\n" % e)
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

# **recordings_medium_by_ids**
> List[RecordingMediumDTO] recordings_medium_by_ids(ids, page=page, size=size, sort=sort)

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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    ids = 'GBAHT0108619' # str | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
    page = 0 # int | Zero-based page index (0..N) (optional) (default to 0)
    size = 20 # int | The size of the page to be returned (optional) (default to 20)
    sort = ['sort_example'] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional)

    try:
        # Recordings by IDs with a medium sized response.
        api_response = api_instance.recordings_medium_by_ids(ids, page=page, size=size, sort=sort)
        print("The response of UserApi->recordings_medium_by_ids:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->recordings_medium_by_ids: %s\n" % e)
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

# **sign_up**
> SignUpDTO sign_up(save_user_dto)

Sign up a new user.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.save_user_dto import SaveUserDTO
from songtradr_api_client_python.models.sign_up_dto import SignUpDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    save_user_dto = songtradr_api_client_python.SaveUserDTO() # SaveUserDTO | 

    try:
        # Sign up a new user.
        api_response = api_instance.sign_up(save_user_dto)
        print("The response of UserApi->sign_up:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->sign_up: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **save_user_dto** | [**SaveUserDTO**](SaveUserDTO.md)|  | 

### Return type

[**SignUpDTO**](SignUpDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Signed up a new user. |  -  |
**409** | User identification is not available. |  -  |
**403** | User is not allowed to sign up other users. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **token**
> JwtTokenDTO token(token_request)

Generates a new JWT token for the given refresh token

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.jwt_token_dto import JwtTokenDTO
from songtradr_api_client_python.models.token_request import TokenRequest
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    token_request = songtradr_api_client_python.TokenRequest() # TokenRequest | 

    try:
        # Generates a new JWT token for the given refresh token
        api_response = api_instance.token(token_request)
        print("The response of UserApi->token:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->token: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **token_request** | [**TokenRequest**](TokenRequest.md)|  | 

### Return type

[**JwtTokenDTO**](JwtTokenDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Generated a bearer JWT token |  -  |
**401** | The given refresh token is invalid or expired |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **update_password**
> object update_password(update_password_dto)

Update password by using the password reset token

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.update_password_dto import UpdatePasswordDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    update_password_dto = songtradr_api_client_python.UpdatePasswordDTO() # UpdatePasswordDTO | 

    try:
        # Update password by using the password reset token
        api_response = api_instance.update_password(update_password_dto)
        print("The response of UserApi->update_password:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->update_password: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **update_password_dto** | [**UpdatePasswordDTO**](UpdatePasswordDTO.md)|  | 

### Return type

**object**

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/hal+json, application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**204** | Password was updated |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |
**400** | Bad Request |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **user_file**
> FileWIthUrlDTO user_file(object_key)

Details and a download link for a file.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.file_w_ith_url_dto import FileWIthUrlDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    object_key = '73818371-0963-412e-aa3d-27c2bab952a3' # str | ObjectKey of the file that should be edited.

    try:
        # Details and a download link for a file.
        api_response = api_instance.user_file(object_key)
        print("The response of UserApi->user_file:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->user_file: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_key** | **str**| ObjectKey of the file that should be edited. | 

### Return type

[**FileWIthUrlDTO**](FileWIthUrlDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Found file. |  -  |
**400** | File not found with this objectKey. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **user_files**
> FileListDTO user_files(isrc=isrc, contributor=contributor, main_artist=main_artist, composer=composer, title=title, party_and_title=party_and_title, language=language, genre_names=genre_names, tag_names=tag_names, release_date=release_date, primary_mood_cluster=primary_mood_cluster, secondary_mood_cluster=secondary_mood_cluster, tertiary_mood_cluster=tertiary_mood_cluster, valence=valence, arousal=arousal, pleasantness=pleasantness, engagement=engagement, vocals=vocals, dominant_instrument=dominant_instrument, secondary_instrument=secondary_instrument, tertiary_instrument=tertiary_instrument, energy=energy, sound_generation=sound_generation, tempo=tempo, scale=scale, key=key, rhythm=rhythm, primary_sound_character=primary_sound_character, timbre=timbre, roughness=roughness, tonality=tonality, harmony=harmony, texture=texture, groovyness=groovyness, space=space, loudness=loudness, production_rating=production_rating, performance_rating=performance_rating, song_rating=song_rating, audience_age=audience_age, audience_region=audience_region, audience_gender=audience_gender, origin_decade=origin_decade, curateability=curateability, use_case=use_case, channel_suitability=channel_suitability, pretzel_station_suitability=pretzel_station_suitability, similar_to_recording=similar_to_recording, songtradr_track_id=songtradr_track_id, usage_name=usage_name, bpm_min=bpm_min, bpm_max=bpm_max, name=name, folder=folder, extension=extension, upload_end_time=upload_end_time, min_upload_end_time=min_upload_end_time, max_upload_end_time=max_upload_end_time, fingerprint_status=fingerprint_status, inference_status=inference_status, page=page, size=size, sort=sort)

List and search your own files.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.file_list_dto import FileListDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    isrc = 'USUM71703692' # str | Search for a ISRC (optional)
    contributor = 'Rick Rubin' # str | Search for a name that was involved as any contributor. (optional)
    main_artist = 'The Beatles' # str | Search for a main artist. (optional)
    composer = 'John Cale' # str | Search for a composer. (optional)
    title = 'Highway To Hell' # str | Search for a title. (optional)
    party_and_title = 'The Beatles yesterday' # str | Search for party and title. (optional)
    language = 'language_example' # str | Search for a language of the lyrics. (optional)
    genre_names = ['genre_names_example'] # List[str] |  (optional)
    tag_names = ['tag_names_example'] # List[str] |  (optional)
    release_date = '2013-10-20T19:20:30+01:00' # datetime |  (optional)
    primary_mood_cluster = 'primary_mood_cluster_example' # str |  (optional)
    secondary_mood_cluster = 'secondary_mood_cluster_example' # str |  (optional)
    tertiary_mood_cluster = 'tertiary_mood_cluster_example' # str |  (optional)
    valence = 'valence_example' # str |  (optional)
    arousal = 'arousal_example' # str |  (optional)
    pleasantness = 'pleasantness_example' # str |  (optional)
    engagement = 'engagement_example' # str |  (optional)
    vocals = 'vocals_example' # str |  (optional)
    dominant_instrument = 'dominant_instrument_example' # str |  (optional)
    secondary_instrument = 'secondary_instrument_example' # str |  (optional)
    tertiary_instrument = 'tertiary_instrument_example' # str |  (optional)
    energy = 'energy_example' # str |  (optional)
    sound_generation = 'sound_generation_example' # str |  (optional)
    tempo = 'tempo_example' # str |  (optional)
    scale = 'scale_example' # str |  (optional)
    key = 'key_example' # str |  (optional)
    rhythm = 'rhythm_example' # str |  (optional)
    primary_sound_character = 'primary_sound_character_example' # str |  (optional)
    timbre = 'timbre_example' # str |  (optional)
    roughness = 'roughness_example' # str |  (optional)
    tonality = 'tonality_example' # str |  (optional)
    harmony = 'harmony_example' # str |  (optional)
    texture = 'texture_example' # str |  (optional)
    groovyness = 'groovyness_example' # str |  (optional)
    space = 'space_example' # str |  (optional)
    loudness = 'loudness_example' # str |  (optional)
    production_rating = 'production_rating_example' # str |  (optional)
    performance_rating = 'performance_rating_example' # str |  (optional)
    song_rating = 'song_rating_example' # str |  (optional)
    audience_age = 'audience_age_example' # str |  (optional)
    audience_region = 'audience_region_example' # str |  (optional)
    audience_gender = 'audience_gender_example' # str |  (optional)
    origin_decade = 'origin_decade_example' # str |  (optional)
    curateability = 'curateability_example' # str |  (optional)
    use_case = 'use_case_example' # str |  (optional)
    channel_suitability = 'channel_suitability_example' # str |  (optional)
    pretzel_station_suitability = 'pretzel_station_suitability_example' # str |  (optional)
    similar_to_recording = 'similar_to_recording_example' # str |  (optional)
    songtradr_track_id = 'songtradr_track_id_example' # str |  (optional)
    usage_name = 'usage_name_example' # str |  (optional)
    bpm_min = 50 # int | Search for a minimal bpm. (optional)
    bpm_max = 210 # int | Search for a maximal bpm. (optional)
    name = 'Groove.mp3' # str | Search for a file name. (optional)
    folder = 'defaultFolder' # str | Search for a folder. (optional)
    extension = '.mp3' # str | Search for a file extension. (optional)
    upload_end_time = '2013-10-20T19:20:30+01:00' # datetime |  (optional)
    min_upload_end_time = '2013-10-20T19:20:30+01:00' # datetime |  (optional)
    max_upload_end_time = '2013-10-20T19:20:30+01:00' # datetime |  (optional)
    fingerprint_status = 'done' # str | Search for a fingerprint status. (optional)
    inference_status = 'done' # str | Search for a inference status. (optional)
    page = 0 # int | Zero-based page index (0..N) (optional) (default to 0)
    size = 100 # int | The size of the page to be returned (optional) (default to 100)
    sort = ["uploadStartTime,DESC"] # List[str] | Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. (optional) (default to ["uploadStartTime,DESC"])

    try:
        # List and search your own files.
        api_response = api_instance.user_files(isrc=isrc, contributor=contributor, main_artist=main_artist, composer=composer, title=title, party_and_title=party_and_title, language=language, genre_names=genre_names, tag_names=tag_names, release_date=release_date, primary_mood_cluster=primary_mood_cluster, secondary_mood_cluster=secondary_mood_cluster, tertiary_mood_cluster=tertiary_mood_cluster, valence=valence, arousal=arousal, pleasantness=pleasantness, engagement=engagement, vocals=vocals, dominant_instrument=dominant_instrument, secondary_instrument=secondary_instrument, tertiary_instrument=tertiary_instrument, energy=energy, sound_generation=sound_generation, tempo=tempo, scale=scale, key=key, rhythm=rhythm, primary_sound_character=primary_sound_character, timbre=timbre, roughness=roughness, tonality=tonality, harmony=harmony, texture=texture, groovyness=groovyness, space=space, loudness=loudness, production_rating=production_rating, performance_rating=performance_rating, song_rating=song_rating, audience_age=audience_age, audience_region=audience_region, audience_gender=audience_gender, origin_decade=origin_decade, curateability=curateability, use_case=use_case, channel_suitability=channel_suitability, pretzel_station_suitability=pretzel_station_suitability, similar_to_recording=similar_to_recording, songtradr_track_id=songtradr_track_id, usage_name=usage_name, bpm_min=bpm_min, bpm_max=bpm_max, name=name, folder=folder, extension=extension, upload_end_time=upload_end_time, min_upload_end_time=min_upload_end_time, max_upload_end_time=max_upload_end_time, fingerprint_status=fingerprint_status, inference_status=inference_status, page=page, size=size, sort=sort)
        print("The response of UserApi->user_files:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->user_files: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **isrc** | **str**| Search for a ISRC | [optional] 
 **contributor** | **str**| Search for a name that was involved as any contributor. | [optional] 
 **main_artist** | **str**| Search for a main artist. | [optional] 
 **composer** | **str**| Search for a composer. | [optional] 
 **title** | **str**| Search for a title. | [optional] 
 **party_and_title** | **str**| Search for party and title. | [optional] 
 **language** | **str**| Search for a language of the lyrics. | [optional] 
 **genre_names** | [**List[str]**](str.md)|  | [optional] 
 **tag_names** | [**List[str]**](str.md)|  | [optional] 
 **release_date** | **datetime**|  | [optional] 
 **primary_mood_cluster** | **str**|  | [optional] 
 **secondary_mood_cluster** | **str**|  | [optional] 
 **tertiary_mood_cluster** | **str**|  | [optional] 
 **valence** | **str**|  | [optional] 
 **arousal** | **str**|  | [optional] 
 **pleasantness** | **str**|  | [optional] 
 **engagement** | **str**|  | [optional] 
 **vocals** | **str**|  | [optional] 
 **dominant_instrument** | **str**|  | [optional] 
 **secondary_instrument** | **str**|  | [optional] 
 **tertiary_instrument** | **str**|  | [optional] 
 **energy** | **str**|  | [optional] 
 **sound_generation** | **str**|  | [optional] 
 **tempo** | **str**|  | [optional] 
 **scale** | **str**|  | [optional] 
 **key** | **str**|  | [optional] 
 **rhythm** | **str**|  | [optional] 
 **primary_sound_character** | **str**|  | [optional] 
 **timbre** | **str**|  | [optional] 
 **roughness** | **str**|  | [optional] 
 **tonality** | **str**|  | [optional] 
 **harmony** | **str**|  | [optional] 
 **texture** | **str**|  | [optional] 
 **groovyness** | **str**|  | [optional] 
 **space** | **str**|  | [optional] 
 **loudness** | **str**|  | [optional] 
 **production_rating** | **str**|  | [optional] 
 **performance_rating** | **str**|  | [optional] 
 **song_rating** | **str**|  | [optional] 
 **audience_age** | **str**|  | [optional] 
 **audience_region** | **str**|  | [optional] 
 **audience_gender** | **str**|  | [optional] 
 **origin_decade** | **str**|  | [optional] 
 **curateability** | **str**|  | [optional] 
 **use_case** | **str**|  | [optional] 
 **channel_suitability** | **str**|  | [optional] 
 **pretzel_station_suitability** | **str**|  | [optional] 
 **similar_to_recording** | **str**|  | [optional] 
 **songtradr_track_id** | **str**|  | [optional] 
 **usage_name** | **str**|  | [optional] 
 **bpm_min** | **int**| Search for a minimal bpm. | [optional] 
 **bpm_max** | **int**| Search for a maximal bpm. | [optional] 
 **name** | **str**| Search for a file name. | [optional] 
 **folder** | **str**| Search for a folder. | [optional] 
 **extension** | **str**| Search for a file extension. | [optional] 
 **upload_end_time** | **datetime**|  | [optional] 
 **min_upload_end_time** | **datetime**|  | [optional] 
 **max_upload_end_time** | **datetime**|  | [optional] 
 **fingerprint_status** | **str**| Search for a fingerprint status. | [optional] 
 **inference_status** | **str**| Search for a inference status. | [optional] 
 **page** | **int**| Zero-based page index (0..N) | [optional] [default to 0]
 **size** | **int**| The size of the page to be returned | [optional] [default to 100]
 **sort** | [**List[str]**](str.md)| Sorting criteria in the format: property,(asc|desc). Default sort order is ascending. Multiple sort criteria are supported. | [optional] [default to [&quot;uploadStartTime,DESC&quot;]]

### Return type

[**FileListDTO**](FileListDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | found files. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **user_files_status**
> List[FileSmallDTO] user_files_status(object_keys)

Status details for files.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.file_small_dto import FileSmallDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    object_keys = 'Example-objectKey' # str | Comma-separated  list of objectKeys of the files.

    try:
        # Status details for files.
        api_response = api_instance.user_files_status(object_keys)
        print("The response of UserApi->user_files_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->user_files_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **object_keys** | **str**| Comma-separated  list of objectKeys of the files. | 

### Return type

[**List[FileSmallDTO]**](FileSmallDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Found files. |  -  |
**400** | File not found with this objectKey. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **user_files_summary**
> FilesSummaryDTO user_files_summary(isrc=isrc, contributor=contributor, main_artist=main_artist, composer=composer, title=title, language=language, genre_names=genre_names, tag_names=tag_names, release_date=release_date, primary_mood_cluster=primary_mood_cluster, secondary_mood_cluster=secondary_mood_cluster, tertiary_mood_cluster=tertiary_mood_cluster, valence=valence, arousal=arousal, pleasantness=pleasantness, engagement=engagement, vocals=vocals, dominant_instrument=dominant_instrument, secondary_instrument=secondary_instrument, tertiary_instrument=tertiary_instrument, energy=energy, sound_generation=sound_generation, tempo=tempo, scale=scale, key=key, rhythm=rhythm, primary_sound_character=primary_sound_character, timbre=timbre, roughness=roughness, tonality=tonality, harmony=harmony, texture=texture, groovyness=groovyness, space=space, loudness=loudness, production_rating=production_rating, performance_rating=performance_rating, song_rating=song_rating, audience_age=audience_age, audience_region=audience_region, audience_gender=audience_gender, origin_decade=origin_decade, curateability=curateability, use_case=use_case, channel_suitability=channel_suitability, pretzel_station_suitability=pretzel_station_suitability, similar_to_recording=similar_to_recording, songtradr_track_id=songtradr_track_id, usage_name=usage_name, bpm_min=bpm_min, bpm_max=bpm_max, name=name, folder=folder, extension=extension, upload_end_time=upload_end_time, min_upload_end_time=min_upload_end_time, max_upload_end_time=max_upload_end_time, fingerprint_status=fingerprint_status, inference_status=inference_status)

Summary fo your files.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.files_summary_dto import FilesSummaryDTO
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
    api_instance = songtradr_api_client_python.UserApi(api_client)
    isrc = 'USUM71703692' # str | Search for a ISRC (optional)
    contributor = 'Rick Rubin' # str | Search for a name that was involved as any contributor. (optional)
    main_artist = 'The Beatles' # str | Search for a main artist. (optional)
    composer = 'John Cale' # str | Search for a composer. (optional)
    title = 'Highway To Hell' # str | Search for a title. (optional)
    language = 'language_example' # str | Search for a language of the lyrics. (optional)
    genre_names = ['genre_names_example'] # List[str] |  (optional)
    tag_names = ['tag_names_example'] # List[str] |  (optional)
    release_date = '2013-10-20T19:20:30+01:00' # datetime |  (optional)
    primary_mood_cluster = 'primary_mood_cluster_example' # str |  (optional)
    secondary_mood_cluster = 'secondary_mood_cluster_example' # str |  (optional)
    tertiary_mood_cluster = 'tertiary_mood_cluster_example' # str |  (optional)
    valence = 'valence_example' # str |  (optional)
    arousal = 'arousal_example' # str |  (optional)
    pleasantness = 'pleasantness_example' # str |  (optional)
    engagement = 'engagement_example' # str |  (optional)
    vocals = 'vocals_example' # str |  (optional)
    dominant_instrument = 'dominant_instrument_example' # str |  (optional)
    secondary_instrument = 'secondary_instrument_example' # str |  (optional)
    tertiary_instrument = 'tertiary_instrument_example' # str |  (optional)
    energy = 'energy_example' # str |  (optional)
    sound_generation = 'sound_generation_example' # str |  (optional)
    tempo = 'tempo_example' # str |  (optional)
    scale = 'scale_example' # str |  (optional)
    key = 'key_example' # str |  (optional)
    rhythm = 'rhythm_example' # str |  (optional)
    primary_sound_character = 'primary_sound_character_example' # str |  (optional)
    timbre = 'timbre_example' # str |  (optional)
    roughness = 'roughness_example' # str |  (optional)
    tonality = 'tonality_example' # str |  (optional)
    harmony = 'harmony_example' # str |  (optional)
    texture = 'texture_example' # str |  (optional)
    groovyness = 'groovyness_example' # str |  (optional)
    space = 'space_example' # str |  (optional)
    loudness = 'loudness_example' # str |  (optional)
    production_rating = 'production_rating_example' # str |  (optional)
    performance_rating = 'performance_rating_example' # str |  (optional)
    song_rating = 'song_rating_example' # str |  (optional)
    audience_age = 'audience_age_example' # str |  (optional)
    audience_region = 'audience_region_example' # str |  (optional)
    audience_gender = 'audience_gender_example' # str |  (optional)
    origin_decade = 'origin_decade_example' # str |  (optional)
    curateability = 'curateability_example' # str |  (optional)
    use_case = 'use_case_example' # str |  (optional)
    channel_suitability = 'channel_suitability_example' # str |  (optional)
    pretzel_station_suitability = 'pretzel_station_suitability_example' # str |  (optional)
    similar_to_recording = 'Highway To Hell' # str |  (optional)
    songtradr_track_id = 'songtradr_track_id_example' # str |  (optional)
    usage_name = 'usage_name_example' # str |  (optional)
    bpm_min = 50 # int | Search for a minimal bpm. (optional)
    bpm_max = 210 # int | Search for a maximal bpm. (optional)
    name = 'Groove.mp3' # str | Search for a file name. (optional)
    folder = 'defaultFolder' # str | Search for a folder. (optional)
    extension = '.mp3' # str | Search for a file extension. (optional)
    upload_end_time = '2013-10-20T19:20:30+01:00' # datetime |  (optional)
    min_upload_end_time = '2013-10-20T19:20:30+01:00' # datetime |  (optional)
    max_upload_end_time = '2013-10-20T19:20:30+01:00' # datetime |  (optional)
    fingerprint_status = 'done' # str | Search for a fingerprint status. (optional)
    inference_status = 'done' # str | Search for a inference status. (optional)

    try:
        # Summary fo your files.
        api_response = api_instance.user_files_summary(isrc=isrc, contributor=contributor, main_artist=main_artist, composer=composer, title=title, language=language, genre_names=genre_names, tag_names=tag_names, release_date=release_date, primary_mood_cluster=primary_mood_cluster, secondary_mood_cluster=secondary_mood_cluster, tertiary_mood_cluster=tertiary_mood_cluster, valence=valence, arousal=arousal, pleasantness=pleasantness, engagement=engagement, vocals=vocals, dominant_instrument=dominant_instrument, secondary_instrument=secondary_instrument, tertiary_instrument=tertiary_instrument, energy=energy, sound_generation=sound_generation, tempo=tempo, scale=scale, key=key, rhythm=rhythm, primary_sound_character=primary_sound_character, timbre=timbre, roughness=roughness, tonality=tonality, harmony=harmony, texture=texture, groovyness=groovyness, space=space, loudness=loudness, production_rating=production_rating, performance_rating=performance_rating, song_rating=song_rating, audience_age=audience_age, audience_region=audience_region, audience_gender=audience_gender, origin_decade=origin_decade, curateability=curateability, use_case=use_case, channel_suitability=channel_suitability, pretzel_station_suitability=pretzel_station_suitability, similar_to_recording=similar_to_recording, songtradr_track_id=songtradr_track_id, usage_name=usage_name, bpm_min=bpm_min, bpm_max=bpm_max, name=name, folder=folder, extension=extension, upload_end_time=upload_end_time, min_upload_end_time=min_upload_end_time, max_upload_end_time=max_upload_end_time, fingerprint_status=fingerprint_status, inference_status=inference_status)
        print("The response of UserApi->user_files_summary:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UserApi->user_files_summary: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **isrc** | **str**| Search for a ISRC | [optional] 
 **contributor** | **str**| Search for a name that was involved as any contributor. | [optional] 
 **main_artist** | **str**| Search for a main artist. | [optional] 
 **composer** | **str**| Search for a composer. | [optional] 
 **title** | **str**| Search for a title. | [optional] 
 **language** | **str**| Search for a language of the lyrics. | [optional] 
 **genre_names** | [**List[str]**](str.md)|  | [optional] 
 **tag_names** | [**List[str]**](str.md)|  | [optional] 
 **release_date** | **datetime**|  | [optional] 
 **primary_mood_cluster** | **str**|  | [optional] 
 **secondary_mood_cluster** | **str**|  | [optional] 
 **tertiary_mood_cluster** | **str**|  | [optional] 
 **valence** | **str**|  | [optional] 
 **arousal** | **str**|  | [optional] 
 **pleasantness** | **str**|  | [optional] 
 **engagement** | **str**|  | [optional] 
 **vocals** | **str**|  | [optional] 
 **dominant_instrument** | **str**|  | [optional] 
 **secondary_instrument** | **str**|  | [optional] 
 **tertiary_instrument** | **str**|  | [optional] 
 **energy** | **str**|  | [optional] 
 **sound_generation** | **str**|  | [optional] 
 **tempo** | **str**|  | [optional] 
 **scale** | **str**|  | [optional] 
 **key** | **str**|  | [optional] 
 **rhythm** | **str**|  | [optional] 
 **primary_sound_character** | **str**|  | [optional] 
 **timbre** | **str**|  | [optional] 
 **roughness** | **str**|  | [optional] 
 **tonality** | **str**|  | [optional] 
 **harmony** | **str**|  | [optional] 
 **texture** | **str**|  | [optional] 
 **groovyness** | **str**|  | [optional] 
 **space** | **str**|  | [optional] 
 **loudness** | **str**|  | [optional] 
 **production_rating** | **str**|  | [optional] 
 **performance_rating** | **str**|  | [optional] 
 **song_rating** | **str**|  | [optional] 
 **audience_age** | **str**|  | [optional] 
 **audience_region** | **str**|  | [optional] 
 **audience_gender** | **str**|  | [optional] 
 **origin_decade** | **str**|  | [optional] 
 **curateability** | **str**|  | [optional] 
 **use_case** | **str**|  | [optional] 
 **channel_suitability** | **str**|  | [optional] 
 **pretzel_station_suitability** | **str**|  | [optional] 
 **similar_to_recording** | **str**|  | [optional] 
 **songtradr_track_id** | **str**|  | [optional] 
 **usage_name** | **str**|  | [optional] 
 **bpm_min** | **int**| Search for a minimal bpm. | [optional] 
 **bpm_max** | **int**| Search for a maximal bpm. | [optional] 
 **name** | **str**| Search for a file name. | [optional] 
 **folder** | **str**| Search for a folder. | [optional] 
 **extension** | **str**| Search for a file extension. | [optional] 
 **upload_end_time** | **datetime**|  | [optional] 
 **min_upload_end_time** | **datetime**|  | [optional] 
 **max_upload_end_time** | **datetime**|  | [optional] 
 **fingerprint_status** | **str**| Search for a fingerprint status. | [optional] 
 **inference_status** | **str**| Search for a inference status. | [optional] 

### Return type

[**FilesSummaryDTO**](FilesSummaryDTO.md)

### Authorization

[bearer-jwt](../README.md#bearer-jwt)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | found files. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

