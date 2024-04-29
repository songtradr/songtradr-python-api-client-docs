# FileDTO

Details on a file that has been uploaded for auto-tagging or audio-recognition purposes.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**object_key** | **str** |  | 
**folder** | **str** |  | 
**extension** | **str** | extension of the file | 
**url** | **str** |  | [optional] 
**upload_start_time** | **datetime** |  | [optional] 
**upload_end_time** | **datetime** |  | [optional] 
**fingerprint_status** | **str** | status of the audio recognition | [optional] 
**fingerprint_start_time** | **datetime** |  | [optional] 
**fingerprint_end_time** | **datetime** |  | [optional] 
**inference_status** | **str** | status of the auto-tagging | [optional] 
**inference_start_time** | **datetime** |  | [optional] 
**inference_end_time** | **datetime** |  | [optional] 
**recording** | [**RecordingMediumDTO**](RecordingMediumDTO.md) |  | [optional] 
**error_time** | **datetime** |  | [optional] 
**error_message** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.file_dto import FileDTO

# TODO update the JSON string below
json = "{}"
# create an instance of FileDTO from a JSON string
file_dto_instance = FileDTO.from_json(json)
# print the JSON string representation of the object
print(FileDTO.to_json())

# convert the object into a dict
file_dto_dict = file_dto_instance.to_dict()
# create an instance of FileDTO from a dict
file_dto_from_dict = FileDTO.from_dict(file_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


