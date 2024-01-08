# CuratePlaylistResponseDTO


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**songtradr_track_ids** | **List[str]** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.curate_playlist_response_dto import CuratePlaylistResponseDTO

# TODO update the JSON string below
json = "{}"
# create an instance of CuratePlaylistResponseDTO from a JSON string
curate_playlist_response_dto_instance = CuratePlaylistResponseDTO.from_json(json)
# print the JSON string representation of the object
print CuratePlaylistResponseDTO.to_json()

# convert the object into a dict
curate_playlist_response_dto_dict = curate_playlist_response_dto_instance.to_dict()
# create an instance of CuratePlaylistResponseDTO from a dict
curate_playlist_response_dto_form_dict = curate_playlist_response_dto.from_dict(curate_playlist_response_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


