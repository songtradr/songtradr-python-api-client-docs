# SaveRecordingPlaylistDTO

Recording Playlist connection

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**songtradr_track_guid** | **str** |  | 
**assigned_by_id** | **int** |  | 
**sequence** | **int** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.save_recording_playlist_dto import SaveRecordingPlaylistDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SaveRecordingPlaylistDTO from a JSON string
save_recording_playlist_dto_instance = SaveRecordingPlaylistDTO.from_json(json)
# print the JSON string representation of the object
print SaveRecordingPlaylistDTO.to_json()

# convert the object into a dict
save_recording_playlist_dto_dict = save_recording_playlist_dto_instance.to_dict()
# create an instance of SaveRecordingPlaylistDTO from a dict
save_recording_playlist_dto_form_dict = save_recording_playlist_dto.from_dict(save_recording_playlist_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


