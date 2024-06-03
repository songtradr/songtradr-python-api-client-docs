# FileWIthUrlDTO

Details on a file that has been uploaded for auto-tagging or audio-recognition purposes. including download path.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file** | [**FileDTO**](FileDTO.md) |  | 
**url** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.file_w_ith_url_dto import FileWIthUrlDTO

# TODO update the JSON string below
json = "{}"
# create an instance of FileWIthUrlDTO from a JSON string
file_w_ith_url_dto_instance = FileWIthUrlDTO.from_json(json)
# print the JSON string representation of the object
print(FileWIthUrlDTO.to_json())

# convert the object into a dict
file_w_ith_url_dto_dict = file_w_ith_url_dto_instance.to_dict()
# create an instance of FileWIthUrlDTO from a dict
file_w_ith_url_dto_from_dict = FileWIthUrlDTO.from_dict(file_w_ith_url_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


