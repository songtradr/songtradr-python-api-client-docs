# CreateApiKeyDTO


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.create_api_key_dto import CreateApiKeyDTO

# TODO update the JSON string below
json = "{}"
# create an instance of CreateApiKeyDTO from a JSON string
create_api_key_dto_instance = CreateApiKeyDTO.from_json(json)
# print the JSON string representation of the object
print CreateApiKeyDTO.to_json()

# convert the object into a dict
create_api_key_dto_dict = create_api_key_dto_instance.to_dict()
# create an instance of CreateApiKeyDTO from a dict
create_api_key_dto_form_dict = create_api_key_dto.from_dict(create_api_key_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


