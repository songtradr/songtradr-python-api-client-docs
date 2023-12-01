# SearchRecordingGranularDTO

Timeseries of tags.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**strength** | **float** | Strength of presence of the corresponding category, tag or genre. | [optional] 
**tag_name** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.search_recording_granular_dto import SearchRecordingGranularDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SearchRecordingGranularDTO from a JSON string
search_recording_granular_dto_instance = SearchRecordingGranularDTO.from_json(json)
# print the JSON string representation of the object
print SearchRecordingGranularDTO.to_json()

# convert the object into a dict
search_recording_granular_dto_dict = search_recording_granular_dto_instance.to_dict()
# create an instance of SearchRecordingGranularDTO from a dict
search_recording_granular_dto_form_dict = search_recording_granular_dto.from_dict(search_recording_granular_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


