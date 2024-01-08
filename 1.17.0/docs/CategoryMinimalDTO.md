# CategoryMinimalDTO

A category of tags in its minimal form.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**category_name** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.category_minimal_dto import CategoryMinimalDTO

# TODO update the JSON string below
json = "{}"
# create an instance of CategoryMinimalDTO from a JSON string
category_minimal_dto_instance = CategoryMinimalDTO.from_json(json)
# print the JSON string representation of the object
print CategoryMinimalDTO.to_json()

# convert the object into a dict
category_minimal_dto_dict = category_minimal_dto_instance.to_dict()
# create an instance of CategoryMinimalDTO from a dict
category_minimal_dto_form_dict = category_minimal_dto.from_dict(category_minimal_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


