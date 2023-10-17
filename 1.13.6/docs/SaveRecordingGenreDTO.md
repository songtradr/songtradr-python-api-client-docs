# SaveRecordingGenreDTO

Recording-genre-connections to save via the API.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**genre_name** | **str** |  | 
**genre_type** | **str** |  | [optional] 
**affinity** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.save_recording_genre_dto import SaveRecordingGenreDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SaveRecordingGenreDTO from a JSON string
save_recording_genre_dto_instance = SaveRecordingGenreDTO.from_json(json)
# print the JSON string representation of the object
print SaveRecordingGenreDTO.to_json()

# convert the object into a dict
save_recording_genre_dto_dict = save_recording_genre_dto_instance.to_dict()
# create an instance of SaveRecordingGenreDTO from a dict
save_recording_genre_dto_form_dict = save_recording_genre_dto.from_dict(save_recording_genre_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


