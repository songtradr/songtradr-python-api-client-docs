# TagDTO

A tag for recordings.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**categories** | [**List[CategoryMinimalDTO]**](CategoryMinimalDTO.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.tag_dto import TagDTO

# TODO update the JSON string below
json = "{}"
# create an instance of TagDTO from a JSON string
tag_dto_instance = TagDTO.from_json(json)
# print the JSON string representation of the object
print(TagDTO.to_json())

# convert the object into a dict
tag_dto_dict = tag_dto_instance.to_dict()
# create an instance of TagDTO from a dict
tag_dto_from_dict = TagDTO.from_dict(tag_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


