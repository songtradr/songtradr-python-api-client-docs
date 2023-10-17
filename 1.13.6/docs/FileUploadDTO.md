# FileUploadDTO

Details on content, ownership, purpose and access rights of a file to be uploaded.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identifiers** | [**List[ConfigIdentifierDTO]**](ConfigIdentifierDTO.md) |  | [optional] 
**flags** | **List[str]** |  | [optional] 
**access** | [**List[ConfigAccessDTO]**](ConfigAccessDTO.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.file_upload_dto import FileUploadDTO

# TODO update the JSON string below
json = "{}"
# create an instance of FileUploadDTO from a JSON string
file_upload_dto_instance = FileUploadDTO.from_json(json)
# print the JSON string representation of the object
print FileUploadDTO.to_json()

# convert the object into a dict
file_upload_dto_dict = file_upload_dto_instance.to_dict()
# create an instance of FileUploadDTO from a dict
file_upload_dto_form_dict = file_upload_dto.from_dict(file_upload_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


