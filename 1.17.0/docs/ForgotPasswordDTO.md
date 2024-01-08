# ForgotPasswordDTO


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_or_username** | **str** |  | 
**system** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.forgot_password_dto import ForgotPasswordDTO

# TODO update the JSON string below
json = "{}"
# create an instance of ForgotPasswordDTO from a JSON string
forgot_password_dto_instance = ForgotPasswordDTO.from_json(json)
# print the JSON string representation of the object
print ForgotPasswordDTO.to_json()

# convert the object into a dict
forgot_password_dto_dict = forgot_password_dto_instance.to_dict()
# create an instance of ForgotPasswordDTO from a dict
forgot_password_dto_form_dict = forgot_password_dto.from_dict(forgot_password_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


