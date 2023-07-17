# RecordingTagSmallDTO

Tag information in with a small field-set.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tag** | [**TagDTO**](TagDTO.md) |  | 

## Example

```python
from songtradr_api_client_python.models.recording_tag_small_dto import RecordingTagSmallDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingTagSmallDTO from a JSON string
recording_tag_small_dto_instance = RecordingTagSmallDTO.from_json(json)
# print the JSON string representation of the object
print RecordingTagSmallDTO.to_json()

# convert the object into a dict
recording_tag_small_dto_dict = recording_tag_small_dto_instance.to_dict()
# create an instance of RecordingTagSmallDTO from a dict
recording_tag_small_dto_form_dict = recording_tag_small_dto.from_dict(recording_tag_small_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


