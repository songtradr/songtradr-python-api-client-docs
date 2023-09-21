# FileSmallDTO

Reduced details on a file that has been uploaded for auto-tagging or audio-recognition purposes.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**id** | **int** |  | 
**extension** | **str** | extension of the file | 
**error_message** | **str** |  | [optional] 
**folder** | **str** |  | 
**object_key** | **str** |  | 
**upload_start_time** | **datetime** |  | [optional] 
**upload_end_time** | **datetime** |  | [optional] 
**fingerprint_start_time** | **datetime** |  | [optional] 
**fingerprint_end_time** | **datetime** |  | [optional] 
**inference_status** | **str** | status of the auto-tagging | [optional] 
**inference_start_time** | **datetime** |  | [optional] 
**inference_end_time** | **datetime** |  | [optional] 
**error_time** | **datetime** |  | [optional] 
**fingerprint_status** | **str** | status of the audio recognition | [optional] 

## Example

```python
from songtradr_api_client_python.models.file_small_dto import FileSmallDTO

# TODO update the JSON string below
json = "{}"
# create an instance of FileSmallDTO from a JSON string
file_small_dto_instance = FileSmallDTO.from_json(json)
# print the JSON string representation of the object
print FileSmallDTO.to_json()

# convert the object into a dict
file_small_dto_dict = file_small_dto_instance.to_dict()
# create an instance of FileSmallDTO from a dict
file_small_dto_form_dict = file_small_dto.from_dict(file_small_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


