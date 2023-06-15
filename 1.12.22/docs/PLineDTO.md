# PLineDTO

Details on a recording's or product's rights.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**year** | **int** |  | [optional] 
**text** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.p_line_dto import PLineDTO

# TODO update the JSON string below
json = "{}"
# create an instance of PLineDTO from a JSON string
p_line_dto_instance = PLineDTO.from_json(json)
# print the JSON string representation of the object
print PLineDTO.to_json()

# convert the object into a dict
p_line_dto_dict = p_line_dto_instance.to_dict()
# create an instance of PLineDTO from a dict
p_line_dto_form_dict = p_line_dto.from_dict(p_line_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


