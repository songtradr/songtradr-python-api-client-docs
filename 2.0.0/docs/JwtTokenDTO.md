# JwtTokenDTO

Bearer token to be used for authentication.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**jwt_token** | **str** |  | 
**expiration_date** | **datetime** |  | 
**refresh_token** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.jwt_token_dto import JwtTokenDTO

# TODO update the JSON string below
json = "{}"
# create an instance of JwtTokenDTO from a JSON string
jwt_token_dto_instance = JwtTokenDTO.from_json(json)
# print the JSON string representation of the object
print(JwtTokenDTO.to_json())

# convert the object into a dict
jwt_token_dto_dict = jwt_token_dto_instance.to_dict()
# create an instance of JwtTokenDTO from a dict
jwt_token_dto_form_dict = jwt_token_dto.from_dict(jwt_token_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


