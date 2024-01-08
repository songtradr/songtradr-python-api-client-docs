# CategoryMediumDTO

A category of tags with its underlying tags.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 
**tags** | [**List[TagSmallDTO]**](TagSmallDTO.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.category_medium_dto import CategoryMediumDTO

# TODO update the JSON string below
json = "{}"
# create an instance of CategoryMediumDTO from a JSON string
category_medium_dto_instance = CategoryMediumDTO.from_json(json)
# print the JSON string representation of the object
print CategoryMediumDTO.to_json()

# convert the object into a dict
category_medium_dto_dict = category_medium_dto_instance.to_dict()
# create an instance of CategoryMediumDTO from a dict
category_medium_dto_form_dict = category_medium_dto.from_dict(category_medium_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


