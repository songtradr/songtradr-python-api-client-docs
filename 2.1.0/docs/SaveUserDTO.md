# SaveUserDTO

Credentials for sign-up to musicube the API and Website.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**system** | **str** |  | [optional] 
**email_address** | **str** |  | 
**password** | **str** |  | [optional] 
**full_name** | **str** |  | [optional] 
**company_name** | **str** |  | [optional] 
**language** | **str** | Current status of the recording. | [optional] 

## Example

```python
from songtradr_api_client_python.models.save_user_dto import SaveUserDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SaveUserDTO from a JSON string
save_user_dto_instance = SaveUserDTO.from_json(json)
# print the JSON string representation of the object
print(SaveUserDTO.to_json())

# convert the object into a dict
save_user_dto_dict = save_user_dto_instance.to_dict()
# create an instance of SaveUserDTO from a dict
save_user_dto_from_dict = SaveUserDTO.from_dict(save_user_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


