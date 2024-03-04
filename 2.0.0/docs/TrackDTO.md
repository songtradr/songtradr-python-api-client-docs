# TrackDTO

A track that connects from recording to a product with a mid-sized field set.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**songtradr_track_id** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.track_dto import TrackDTO

# TODO update the JSON string below
json = "{}"
# create an instance of TrackDTO from a JSON string
track_dto_instance = TrackDTO.from_json(json)
# print the JSON string representation of the object
print(TrackDTO.to_json())

# convert the object into a dict
track_dto_dict = track_dto_instance.to_dict()
# create an instance of TrackDTO from a dict
track_dto_form_dict = track_dto.from_dict(track_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


