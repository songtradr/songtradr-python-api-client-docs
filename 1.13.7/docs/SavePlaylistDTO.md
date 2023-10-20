# SavePlaylistDTO

Save a playlist

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**songtradr_playlist_guid** | **str** |  | 
**name** | **str** |  | 
**description** | **str** |  | [optional] 
**state** | **str** |  | 
**asset_url** | **str** |  | [optional] 
**pretzel_tier** | **str** |  | [optional] 
**usage** | **str** |  | [optional] 
**usages** | **List[str]** |  | 
**recordings** | [**List[SaveRecordingPlaylistDTO]**](SaveRecordingPlaylistDTO.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.save_playlist_dto import SavePlaylistDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SavePlaylistDTO from a JSON string
save_playlist_dto_instance = SavePlaylistDTO.from_json(json)
# print the JSON string representation of the object
print SavePlaylistDTO.to_json()

# convert the object into a dict
save_playlist_dto_dict = save_playlist_dto_instance.to_dict()
# create an instance of SavePlaylistDTO from a dict
save_playlist_dto_form_dict = save_playlist_dto.from_dict(save_playlist_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


