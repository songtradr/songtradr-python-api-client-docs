# CuratePlaylistDTO


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**request_data** | **List[str]** |  | [optional] 
**usage_filter** | **str** |  | [optional] 
**numerical_filter** | **Dict[str, str]** |  | [optional] 
**category_filter** | **Dict[str, str]** |  | [optional] 
**first_id** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.curate_playlist_dto import CuratePlaylistDTO

# TODO update the JSON string below
json = "{}"
# create an instance of CuratePlaylistDTO from a JSON string
curate_playlist_dto_instance = CuratePlaylistDTO.from_json(json)
# print the JSON string representation of the object
print CuratePlaylistDTO.to_json()

# convert the object into a dict
curate_playlist_dto_dict = curate_playlist_dto_instance.to_dict()
# create an instance of CuratePlaylistDTO from a dict
curate_playlist_dto_form_dict = curate_playlist_dto.from_dict(curate_playlist_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


