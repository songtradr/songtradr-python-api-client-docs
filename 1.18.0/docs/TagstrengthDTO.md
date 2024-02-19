# TagstrengthDTO

A TaggramDTO for recordings.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**strength** | **float** | Strength of presence of the corresponding category, tag or genre. | 
**category_name** | **str** |  | 
**tag_name** | **str** |  | [optional] 
**genre_name** | **str** |  | [optional] 
**scale** | **List[int]** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.tagstrength_dto import TagstrengthDTO

# TODO update the JSON string below
json = "{}"
# create an instance of TagstrengthDTO from a JSON string
tagstrength_dto_instance = TagstrengthDTO.from_json(json)
# print the JSON string representation of the object
print TagstrengthDTO.to_json()

# convert the object into a dict
tagstrength_dto_dict = tagstrength_dto_instance.to_dict()
# create an instance of TagstrengthDTO from a dict
tagstrength_dto_form_dict = tagstrength_dto.from_dict(tagstrength_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


