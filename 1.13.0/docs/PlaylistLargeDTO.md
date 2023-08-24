# PlaylistLargeDTO

Details on a playlist

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**state** | **str** |  | [optional] 
**description** | **str** |  | [optional] 
**usages** | [**List[UsageDTO]**](UsageDTO.md) |  | [optional] 
**songtradr_playlist_guid** | **str** |  | [optional] 
**asset_url** | **str** |  | [optional] 
**pretzel_tier** | **str** |  | [optional] 
**usage** | **str** |  | [optional] 
**tracks** | [**List[RecordingPlaylistDTO]**](RecordingPlaylistDTO.md) |  | [optional] 
**created** | **datetime** |  | [optional] 
**updated** | **datetime** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.playlist_large_dto import PlaylistLargeDTO

# TODO update the JSON string below
json = "{}"
# create an instance of PlaylistLargeDTO from a JSON string
playlist_large_dto_instance = PlaylistLargeDTO.from_json(json)
# print the JSON string representation of the object
print PlaylistLargeDTO.to_json()

# convert the object into a dict
playlist_large_dto_dict = playlist_large_dto_instance.to_dict()
# create an instance of PlaylistLargeDTO from a dict
playlist_large_dto_form_dict = playlist_large_dto.from_dict(playlist_large_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


