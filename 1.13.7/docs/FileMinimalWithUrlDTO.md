# FileMinimalWithUrlDTO

Minimal infos on a file that has been uploaded for auto-tagging or audio-recognition purposes. including download path.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**file_name** | **str** |  | 
**url** | **str** |  | 
**isrc** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.file_minimal_with_url_dto import FileMinimalWithUrlDTO

# TODO update the JSON string below
json = "{}"
# create an instance of FileMinimalWithUrlDTO from a JSON string
file_minimal_with_url_dto_instance = FileMinimalWithUrlDTO.from_json(json)
# print the JSON string representation of the object
print FileMinimalWithUrlDTO.to_json()

# convert the object into a dict
file_minimal_with_url_dto_dict = file_minimal_with_url_dto_instance.to_dict()
# create an instance of FileMinimalWithUrlDTO from a dict
file_minimal_with_url_dto_form_dict = file_minimal_with_url_dto.from_dict(file_minimal_with_url_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


