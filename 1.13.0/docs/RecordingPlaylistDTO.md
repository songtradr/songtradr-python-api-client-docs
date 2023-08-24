# RecordingPlaylistDTO

Recording Playlist connection

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recording** | [**RecordingMediumDTO**](RecordingMediumDTO.md) |  | [optional] 
**songtradr_track_guid** | **str** |  | [optional] 
**assigned_by_id** | **int** |  | [optional] 
**sequence** | **int** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.recording_playlist_dto import RecordingPlaylistDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingPlaylistDTO from a JSON string
recording_playlist_dto_instance = RecordingPlaylistDTO.from_json(json)
# print the JSON string representation of the object
print RecordingPlaylistDTO.to_json()

# convert the object into a dict
recording_playlist_dto_dict = recording_playlist_dto_instance.to_dict()
# create an instance of RecordingPlaylistDTO from a dict
recording_playlist_dto_form_dict = recording_playlist_dto.from_dict(recording_playlist_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


