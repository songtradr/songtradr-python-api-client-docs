# SignUpDTO

Credentials for sign-up to musicube the API and Website.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email_address** | **str** |  | 
**password** | **str** |  | 
**full_name** | **str** |  | 
**company_name** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.sign_up_dto import SignUpDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SignUpDTO from a JSON string
sign_up_dto_instance = SignUpDTO.from_json(json)
# print the JSON string representation of the object
print SignUpDTO.to_json()

# convert the object into a dict
sign_up_dto_dict = sign_up_dto_instance.to_dict()
# create an instance of SignUpDTO from a dict
sign_up_dto_form_dict = sign_up_dto.from_dict(sign_up_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


