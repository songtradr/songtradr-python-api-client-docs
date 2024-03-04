# TagSmallDTO

A tag for recordings with a reduced field-set.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.tag_small_dto import TagSmallDTO

# TODO update the JSON string below
json = "{}"
# create an instance of TagSmallDTO from a JSON string
tag_small_dto_instance = TagSmallDTO.from_json(json)
# print the JSON string representation of the object
print(TagSmallDTO.to_json())

# convert the object into a dict
tag_small_dto_dict = tag_small_dto_instance.to_dict()
# create an instance of TagSmallDTO from a dict
tag_small_dto_form_dict = tag_small_dto.from_dict(tag_small_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


