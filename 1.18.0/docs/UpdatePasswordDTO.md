# UpdatePasswordDTO


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**token** | **str** |  | 
**password** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.update_password_dto import UpdatePasswordDTO

# TODO update the JSON string below
json = "{}"
# create an instance of UpdatePasswordDTO from a JSON string
update_password_dto_instance = UpdatePasswordDTO.from_json(json)
# print the JSON string representation of the object
print UpdatePasswordDTO.to_json()

# convert the object into a dict
update_password_dto_dict = update_password_dto_instance.to_dict()
# create an instance of UpdatePasswordDTO from a dict
update_password_dto_form_dict = update_password_dto.from_dict(update_password_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


