# ConfigAccessDTO

Specify access rights.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**accessor_id** | **str** | ID of the accessing entity | 
**rights** | **str** | access rights to a resource | 

## Example

```python
from songtradr_api_client_python.models.config_access_dto import ConfigAccessDTO

# TODO update the JSON string below
json = "{}"
# create an instance of ConfigAccessDTO from a JSON string
config_access_dto_instance = ConfigAccessDTO.from_json(json)
# print the JSON string representation of the object
print ConfigAccessDTO.to_json()

# convert the object into a dict
config_access_dto_dict = config_access_dto_instance.to_dict()
# create an instance of ConfigAccessDTO from a dict
config_access_dto_form_dict = config_access_dto.from_dict(config_access_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


