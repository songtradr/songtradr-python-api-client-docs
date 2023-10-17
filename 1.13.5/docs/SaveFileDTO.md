# SaveFileDTO

Extensive details on a file object.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**folder** | **str** |  | [optional] 
**extension** | **str** |  | [optional] 
**object_key** | **str** |  | [optional] 
**customer** | **str** |  | [optional] 
**upload_start_time** | **datetime** |  | [optional] 
**upload_end_time** | **datetime** |  | [optional] 
**fingerprint_status** | **str** |  | [optional] 
**fingerprint_start_time** | **datetime** |  | [optional] 
**fingerprint_end_time** | **datetime** |  | [optional] 
**inference_status** | **str** |  | [optional] 
**inference_start_time** | **datetime** |  | [optional] 
**inference_end_time** | **datetime** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.save_file_dto import SaveFileDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SaveFileDTO from a JSON string
save_file_dto_instance = SaveFileDTO.from_json(json)
# print the JSON string representation of the object
print SaveFileDTO.to_json()

# convert the object into a dict
save_file_dto_dict = save_file_dto_instance.to_dict()
# create an instance of SaveFileDTO from a dict
save_file_dto_form_dict = save_file_dto.from_dict(save_file_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


