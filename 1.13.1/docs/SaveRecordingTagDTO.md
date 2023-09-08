# SaveRecordingTagDTO

Recording-tag-connections the AI predicts and wants to save the API.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**tag_name** | **str** |  | 
**affinity** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.save_recording_tag_dto import SaveRecordingTagDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SaveRecordingTagDTO from a JSON string
save_recording_tag_dto_instance = SaveRecordingTagDTO.from_json(json)
# print the JSON string representation of the object
print SaveRecordingTagDTO.to_json()

# convert the object into a dict
save_recording_tag_dto_dict = save_recording_tag_dto_instance.to_dict()
# create an instance of SaveRecordingTagDTO from a dict
save_recording_tag_dto_form_dict = save_recording_tag_dto.from_dict(save_recording_tag_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


