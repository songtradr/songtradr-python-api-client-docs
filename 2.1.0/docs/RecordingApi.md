# songtradr_api_client_python.RecordingApi

All URIs are relative to *https://api.songtradr.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**prompt_search_recordings**](RecordingApi.md#prompt_search_recordings) | **GET** /api/v1/public/recording/promptSearch | Recordings for query.
[**recordings_by_ids_with_musical_features**](RecordingApi.md#recordings_by_ids_with_musical_features) | **GET** /api/v1/public/recording/{ids}/musicalFeatures | AI generated moods, musical features and more for recordings.
[**recordings_by_ids_with_similarities1**](RecordingApi.md#recordings_by_ids_with_similarities1) | **GET** /api/v1/public/recording/{ids}/similarities | Similar recordings for a list of recordings.
[**recordings_by_ids_with_taggrams1**](RecordingApi.md#recordings_by_ids_with_taggrams1) | **GET** /api/v1/public/recording/{ids}/taggrams | Timeseries of AI generated moods, musical features and more for a list of recordings.
[**recordings_by_ids_with_tagstrengths1**](RecordingApi.md#recordings_by_ids_with_tagstrengths1) | **GET** /api/v1/public/recording/{ids}/tagstrengths | Strengths as numerical representations for AI generated moods, musical features and more for recordings.
[**recordings_medium_by_ids1**](RecordingApi.md#recordings_medium_by_ids1) | **GET** /api/v1/public/recording/m/{ids} | Recordings by IDs with a medium sized response.
[**search_recordings**](RecordingApi.md#search_recordings) | **GET** /api/v1/public/recording/search | Recordings by contributors, moods, musical features and more.


# **prompt_search_recordings**
> RecordingListDTO prompt_search_recordings(query)

Recordings for query.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.recording_list_dto import RecordingListDTO
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
    query = 'funk, guitar, drums' # str | Query.

    try:
        # Recordings for query.
        api_response = api_instance.prompt_search_recordings(query)
        print("The response of RecordingApi->prompt_search_recordings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordingApi->prompt_search_recordings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query** | **str**| Query. | 

### Return type

[**RecordingListDTO**](RecordingListDTO.md)

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

# **recordings_by_ids_with_musical_features**
> List[RecordingMinimalWithMusicalFeaturesDTO] recordings_by_ids_with_musical_features(ids)

AI generated moods, musical features and more for recordings.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.recording_minimal_with_musical_features_dto import RecordingMinimalWithMusicalFeaturesDTO
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
    ids = 'ZAA010800469' # str | Comma seperated list of IDs. Can be ISRCs or proprietary IDs

    try:
        # AI generated moods, musical features and more for recordings.
        api_response = api_instance.recordings_by_ids_with_musical_features(ids)
        print("The response of RecordingApi->recordings_by_ids_with_musical_features:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordingApi->recordings_by_ids_with_musical_features: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ids** | **str**| Comma seperated list of IDs. Can be ISRCs or proprietary IDs | 

### Return type

[**List[RecordingMinimalWithMusicalFeaturesDTO]**](RecordingMinimalWithMusicalFeaturesDTO.md)

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

# **recordings_by_ids_with_similarities1**
> List[RecordingForSimilaritySearchDTO] recordings_by_ids_with_similarities1(ids, identical_only=identical_only, usage=usage)

Similar recordings for a list of recordings.

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
    api_instance = songtradr_api_client_python.RecordingApi(api_client)
    ids = 'USUM71703692' # str | Comma seperated list of IDs. Can be ISRCs or proprietary IDs
    identical_only = False # bool | Whether a result list shall include only identical recordings. (optional) (default to False)
    usage = 'usage_example' # str | Filter by recording usage. (optional)

    try:
        # Similar recordings for a list of recordings.
        api_response = api_instance.recordings_by_ids_with_similarities1(ids, identical_only=identical_only, usage=usage)
        print("The response of RecordingApi->recordings_by_ids_with_similarities1:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordingApi->recordings_by_ids_with_similarities1: %s\n" % e)
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
**200** | Found recordings. |  -  |
**401** | Unauthorized |  -  |
**429** | Too Many Requests |  -  |
**500** | Internal Server Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

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

# **search_recordings**
> RecordingListDTO search_recordings(similar_to_recording=similar_to_recording, contributor=contributor, main_artist=main_artist, composer=composer, title=title, party_and_title=party_and_title, language=language, genre=genre, primary_mood_cluster=primary_mood_cluster, valence=valence, arousal=arousal, pleasantness=pleasantness, engagement=engagement, vocals=vocals, dominant_instrument=dominant_instrument, energy=energy, sound_generation=sound_generation, tempo=tempo, scale=scale, key=key, rhythm=rhythm, primary_sound_character=primary_sound_character, timbre=timbre, roughness=roughness, tonality=tonality, harmony=harmony, texture=texture, groovyness=groovyness, space=space, loudness=loudness, origin_decade=origin_decade, curateability=curateability, use_case=use_case, channel_suitability=channel_suitability, songtradr_track_id=songtradr_track_id, usage=usage, pretzel_station_suitability=pretzel_station_suitability, similar_to_songtradr_track_id=similar_to_songtradr_track_id, shuffled=shuffled, sort=sort, page=page, size=size)

Recordings by contributors, moods, musical features and more.

### Example

* Bearer (JWT) Authentication (bearer-jwt):

```python
import songtradr_api_client_python
from songtradr_api_client_python.models.recording_list_dto import RecordingListDTO
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
    similar_to_recording = 'GBUM71110209' # str | Search for songs similar to a recording. (optional)
    contributor = 'Rick Rubin' # str | Search for a name that was involved as any contributor. (optional)
    main_artist = 'The Beatles' # str | Search for a main artist. (optional)
    composer = 'John Cale' # str | Search for a composer. (optional)
    title = 'Highway To Hell' # str | Search for a title. (optional)
    party_and_title = 'The Beatles yesterday' # str | Search for party and title. (optional)
    language = 'language_example' # str | Search for a language of the lyrics. (optional)
    genre = 'Rock' # str | Search for a genre. (optional)
    primary_mood_cluster = 'primary_mood_cluster_example' # str | Search for a mood. (optional)
    valence = 'valence_example' # str | Search for valence. (optional)
    arousal = 'arousal_example' # str | Search for arousal. (optional)
    pleasantness = 'pleasantness_example' # str | Search for pleasantness. (optional)
    engagement = 'engagement_example' # str | Search for an engagement. (optional)
    vocals = 'vocals_example' # str | Search for a vocals gender or instrumental songs. (optional)
    dominant_instrument = 'dominant_instrument_example' # str | Search for a dominant instrument. (optional)
    energy = 'energy_example' # str | Search for energy. (optional)
    sound_generation = 'sound_generation_example' # str | Search for type of sound generation. (optional)
    tempo = 'tempo_example' # str | Search for tempo. (optional)
    scale = 'scale_example' # str | Search for tonal scale. (optional)
    key = 'key_example' # str | Search for harmonic key. (optional)
    rhythm = 'rhythm_example' # str | Search for rhythm. (optional)
    primary_sound_character = 'primary_sound_character_example' # str | Search for a sound character. (optional)
    timbre = 'timbre_example' # str | Search for timbre. (optional)
    roughness = 'roughness_example' # str | Search for roughness. (optional)
    tonality = 'tonality_example' # str | Search for tonality. (optional)
    harmony = 'harmony_example' # str | Search for a degree of harmoniousness. (optional)
    texture = 'texture_example' # str | Search for texture. (optional)
    groovyness = 'groovyness_example' # str | Search for groovyness. (optional)
    space = 'space_example' # str | Search for space. (optional)
    loudness = 'loudness_example' # str | Search for loudness. (optional)
    origin_decade = 'origin_decade_example' # str | Search for origin decade. (optional)
    curateability = 'curateability_example' # str | Search for curateability. (optional)
    use_case = 'use_case_example' # str | Search for use case. (optional)
    channel_suitability = 'channel_suitability_example' # str | Search for channel suitability. (optional)
    songtradr_track_id = 'songtradr_track_id_example' # str | Search for Songtradr track id. (optional)
    usage = 'usage_example' # str | Search for recording usage. (optional)
    pretzel_station_suitability = 'pretzel_station_suitability_example' # str | Search for Pretzel station suitability. (optional)
    similar_to_songtradr_track_id = '1bF118m' # str | Search for songs similar to a recording by songtradr Track Id. (optional)
    shuffled = 'false' # str | Sort the results randomly. (optional) (default to 'false')
    sort = 'popularityDesc' # str | Sort the results. (optional) (default to 'popularityDesc')
    page = 0 # int | Zero-based page index (0..N) (optional) (default to 0)
    size = 20 # int | The size of the page to be returned (optional) (default to 20)

    try:
        # Recordings by contributors, moods, musical features and more.
        api_response = api_instance.search_recordings(similar_to_recording=similar_to_recording, contributor=contributor, main_artist=main_artist, composer=composer, title=title, party_and_title=party_and_title, language=language, genre=genre, primary_mood_cluster=primary_mood_cluster, valence=valence, arousal=arousal, pleasantness=pleasantness, engagement=engagement, vocals=vocals, dominant_instrument=dominant_instrument, energy=energy, sound_generation=sound_generation, tempo=tempo, scale=scale, key=key, rhythm=rhythm, primary_sound_character=primary_sound_character, timbre=timbre, roughness=roughness, tonality=tonality, harmony=harmony, texture=texture, groovyness=groovyness, space=space, loudness=loudness, origin_decade=origin_decade, curateability=curateability, use_case=use_case, channel_suitability=channel_suitability, songtradr_track_id=songtradr_track_id, usage=usage, pretzel_station_suitability=pretzel_station_suitability, similar_to_songtradr_track_id=similar_to_songtradr_track_id, shuffled=shuffled, sort=sort, page=page, size=size)
        print("The response of RecordingApi->search_recordings:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling RecordingApi->search_recordings: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **similar_to_recording** | **str**| Search for songs similar to a recording. | [optional] 
 **contributor** | **str**| Search for a name that was involved as any contributor. | [optional] 
 **main_artist** | **str**| Search for a main artist. | [optional] 
 **composer** | **str**| Search for a composer. | [optional] 
 **title** | **str**| Search for a title. | [optional] 
 **party_and_title** | **str**| Search for party and title. | [optional] 
 **language** | **str**| Search for a language of the lyrics. | [optional] 
 **genre** | **str**| Search for a genre. | [optional] 
 **primary_mood_cluster** | **str**| Search for a mood. | [optional] 
 **valence** | **str**| Search for valence. | [optional] 
 **arousal** | **str**| Search for arousal. | [optional] 
 **pleasantness** | **str**| Search for pleasantness. | [optional] 
 **engagement** | **str**| Search for an engagement. | [optional] 
 **vocals** | **str**| Search for a vocals gender or instrumental songs. | [optional] 
 **dominant_instrument** | **str**| Search for a dominant instrument. | [optional] 
 **energy** | **str**| Search for energy. | [optional] 
 **sound_generation** | **str**| Search for type of sound generation. | [optional] 
 **tempo** | **str**| Search for tempo. | [optional] 
 **scale** | **str**| Search for tonal scale. | [optional] 
 **key** | **str**| Search for harmonic key. | [optional] 
 **rhythm** | **str**| Search for rhythm. | [optional] 
 **primary_sound_character** | **str**| Search for a sound character. | [optional] 
 **timbre** | **str**| Search for timbre. | [optional] 
 **roughness** | **str**| Search for roughness. | [optional] 
 **tonality** | **str**| Search for tonality. | [optional] 
 **harmony** | **str**| Search for a degree of harmoniousness. | [optional] 
 **texture** | **str**| Search for texture. | [optional] 
 **groovyness** | **str**| Search for groovyness. | [optional] 
 **space** | **str**| Search for space. | [optional] 
 **loudness** | **str**| Search for loudness. | [optional] 
 **origin_decade** | **str**| Search for origin decade. | [optional] 
 **curateability** | **str**| Search for curateability. | [optional] 
 **use_case** | **str**| Search for use case. | [optional] 
 **channel_suitability** | **str**| Search for channel suitability. | [optional] 
 **songtradr_track_id** | **str**| Search for Songtradr track id. | [optional] 
 **usage** | **str**| Search for recording usage. | [optional] 
 **pretzel_station_suitability** | **str**| Search for Pretzel station suitability. | [optional] 
 **similar_to_songtradr_track_id** | **str**| Search for songs similar to a recording by songtradr Track Id. | [optional] 
 **shuffled** | **str**| Sort the results randomly. | [optional] [default to &#39;false&#39;]
 **sort** | **str**| Sort the results. | [optional] [default to &#39;popularityDesc&#39;]
 **page** | **int**| Zero-based page index (0..N) | [optional] [default to 0]
 **size** | **int**| The size of the page to be returned | [optional] [default to 20]

### Return type

[**RecordingListDTO**](RecordingListDTO.md)

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

