# InitPutRecordingAudioDTO

Object that specifies where to upload a file so it can be processed.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**isrc** | **str** |  | [optional] 
**object_key** | **str** |  | [optional] 
**url** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.init_put_recording_audio_dto import InitPutRecordingAudioDTO

# TODO update the JSON string below
json = "{}"
# create an instance of InitPutRecordingAudioDTO from a JSON string
init_put_recording_audio_dto_instance = InitPutRecordingAudioDTO.from_json(json)
# print the JSON string representation of the object
print InitPutRecordingAudioDTO.to_json()

# convert the object into a dict
init_put_recording_audio_dto_dict = init_put_recording_audio_dto_instance.to_dict()
# create an instance of InitPutRecordingAudioDTO from a dict
init_put_recording_audio_dto_form_dict = init_put_recording_audio_dto.from_dict(init_put_recording_audio_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


