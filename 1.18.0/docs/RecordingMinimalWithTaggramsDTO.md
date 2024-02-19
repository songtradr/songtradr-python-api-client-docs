# RecordingMinimalWithTaggramsDTO

Recording in its minimal form, but with AI-predicted musical features.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**isrc** | **str** |  | 
**timestamps** | **List[float]** | Points in time in seconds. Each value refers to the taggrams values of the same index. | [optional] 
**taggrams** | [**List[TaggramDTO]**](TaggramDTO.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.recording_minimal_with_taggrams_dto import RecordingMinimalWithTaggramsDTO

# TODO update the JSON string below
json = "{}"
# create an instance of RecordingMinimalWithTaggramsDTO from a JSON string
recording_minimal_with_taggrams_dto_instance = RecordingMinimalWithTaggramsDTO.from_json(json)
# print the JSON string representation of the object
print RecordingMinimalWithTaggramsDTO.to_json()

# convert the object into a dict
recording_minimal_with_taggrams_dto_dict = recording_minimal_with_taggrams_dto_instance.to_dict()
# create an instance of RecordingMinimalWithTaggramsDTO from a dict
recording_minimal_with_taggrams_dto_form_dict = recording_minimal_with_taggrams_dto.from_dict(recording_minimal_with_taggrams_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


