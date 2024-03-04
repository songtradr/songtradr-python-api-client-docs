# ConfigIdentifierDTO

Key-Value Pairs to specify and identifier.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**identifier_type** | **str** |  | 
**identifier_value** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.config_identifier_dto import ConfigIdentifierDTO

# TODO update the JSON string below
json = "{}"
# create an instance of ConfigIdentifierDTO from a JSON string
config_identifier_dto_instance = ConfigIdentifierDTO.from_json(json)
# print the JSON string representation of the object
print(ConfigIdentifierDTO.to_json())

# convert the object into a dict
config_identifier_dto_dict = config_identifier_dto_instance.to_dict()
# create an instance of ConfigIdentifierDTO from a dict
config_identifier_dto_form_dict = config_identifier_dto.from_dict(config_identifier_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


