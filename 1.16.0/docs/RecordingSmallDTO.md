# RecordingSmallDTO

Recording with a small field set.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**duration** | **int** |  | [optional] 
**isrc** | **str** |  | 
**parties** | [**List[RecordingPartyDTO]**](RecordingPartyDTO.md) |  | [optional] 
**titles** | [**List[TitleDTO]**](TitleDTO.md) |  | [optional] 
**tracks** | [**List[TrackDTO]**](TrackDTO.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.recording_small_dto import RecordingSmallDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingSmallDTO from a JSON string
recording_small_dto_instance = RecordingSmallDTO.from_json(json)
# print the JSON string representation of the object
print RecordingSmallDTO.to_json()

# convert the object into a dict
recording_small_dto_dict = recording_small_dto_instance.to_dict()
# create an instance of RecordingSmallDTO from a dict
recording_small_dto_form_dict = recording_small_dto.from_dict(recording_small_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


