# FieldSummaryDTO

Summary of genres occuring in files.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**field_value** | **str** |  | 
**total** | **int** |  | 
**field_name** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.field_summary_dto import FieldSummaryDTO

# TODO update the JSON string below
json = "{}"
# create an instance of FieldSummaryDTO from a JSON string
field_summary_dto_instance = FieldSummaryDTO.from_json(json)
# print the JSON string representation of the object
print(FieldSummaryDTO.to_json())

# convert the object into a dict
field_summary_dto_dict = field_summary_dto_instance.to_dict()
# create an instance of FieldSummaryDTO from a dict
field_summary_dto_from_dict = FieldSummaryDTO.from_dict(field_summary_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


