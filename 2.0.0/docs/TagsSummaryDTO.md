# TagsSummaryDTO

Summary of tags occuring in files.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**categories** | [**List[CategoryMinimalDTO]**](CategoryMinimalDTO.md) |  | [optional] 
**total** | **int** |  | 

## Example

```python
from songtradr_api_client_python.models.tags_summary_dto import TagsSummaryDTO

# TODO update the JSON string below
json = "{}"
# create an instance of TagsSummaryDTO from a JSON string
tags_summary_dto_instance = TagsSummaryDTO.from_json(json)
# print the JSON string representation of the object
print(TagsSummaryDTO.to_json())

# convert the object into a dict
tags_summary_dto_dict = tags_summary_dto_instance.to_dict()
# create an instance of TagsSummaryDTO from a dict
tags_summary_dto_form_dict = tags_summary_dto.from_dict(tags_summary_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


