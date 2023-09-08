# SearchRecordingGranularAbstractionDTO

Timeseries of tags.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**strength** | **float** | Strength of presence of the corresponding category, tag or genre. | [optional] 
**abstraction_name** | **str** | Current status of the recording. | 

## Example

```python
from songtradr_api_client_python.models.search_recording_granular_abstraction_dto import SearchRecordingGranularAbstractionDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SearchRecordingGranularAbstractionDTO from a JSON string
search_recording_granular_abstraction_dto_instance = SearchRecordingGranularAbstractionDTO.from_json(json)
# print the JSON string representation of the object
print SearchRecordingGranularAbstractionDTO.to_json()

# convert the object into a dict
search_recording_granular_abstraction_dto_dict = search_recording_granular_abstraction_dto_instance.to_dict()
# create an instance of SearchRecordingGranularAbstractionDTO from a dict
search_recording_granular_abstraction_dto_form_dict = search_recording_granular_abstraction_dto.from_dict(search_recording_granular_abstraction_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


