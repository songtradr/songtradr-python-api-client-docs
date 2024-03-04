# FileListDTO

List of files.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**files** | [**List[FileDTO]**](FileDTO.md) |  | 
**has_next_page** | **bool** |  | 
**current_page_number** | **int** |  | 
**total_results** | **int** |  | 

## Example

```python
from songtradr_api_client_python.models.file_list_dto import FileListDTO

# TODO update the JSON string below
json = "{}"
# create an instance of FileListDTO from a JSON string
file_list_dto_instance = FileListDTO.from_json(json)
# print the JSON string representation of the object
print(FileListDTO.to_json())

# convert the object into a dict
file_list_dto_dict = file_list_dto_instance.to_dict()
# create an instance of FileListDTO from a dict
file_list_dto_form_dict = file_list_dto.from_dict(file_list_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


