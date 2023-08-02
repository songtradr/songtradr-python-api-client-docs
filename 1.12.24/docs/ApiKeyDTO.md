# ApiKeyDTO


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | 
**last_used_at** | **datetime** |  | [optional] 
**created_at** | **datetime** |  | 
**id** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.api_key_dto import ApiKeyDTO

# TODO update the JSON string below
json = "{}"
# create an instance of ApiKeyDTO from a JSON string
api_key_dto_instance = ApiKeyDTO.from_json(json)
# print the JSON string representation of the object
print ApiKeyDTO.to_json()

# convert the object into a dict
api_key_dto_dict = api_key_dto_instance.to_dict()
# create an instance of ApiKeyDTO from a dict
api_key_dto_form_dict = api_key_dto.from_dict(api_key_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


