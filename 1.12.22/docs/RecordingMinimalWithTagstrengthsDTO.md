# RecordingMinimalWithTagstrengthsDTO

Recording in its minimal form, but with AI-predicted musical features.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**isrc** | **str** |  | 
**tagstrengths** | [**List[TagstrengthDTO]**](TagstrengthDTO.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.recording_minimal_with_tagstrengths_dto import RecordingMinimalWithTagstrengthsDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingMinimalWithTagstrengthsDTO from a JSON string
recording_minimal_with_tagstrengths_dto_instance = RecordingMinimalWithTagstrengthsDTO.from_json(json)
# print the JSON string representation of the object
print RecordingMinimalWithTagstrengthsDTO.to_json()

# convert the object into a dict
recording_minimal_with_tagstrengths_dto_dict = recording_minimal_with_tagstrengths_dto_instance.to_dict()
# create an instance of RecordingMinimalWithTagstrengthsDTO from a dict
recording_minimal_with_tagstrengths_dto_form_dict = recording_minimal_with_tagstrengths_dto.from_dict(recording_minimal_with_tagstrengths_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


