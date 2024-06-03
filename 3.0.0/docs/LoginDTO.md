# LoginDTO

Credentials to be used to retrieve bearer token for authentication.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**username** | **str** |  | [optional] 
**version** | **str** |  | [optional] 
**email** | **str** |  | 
**password** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.login_dto import LoginDTO

# TODO update the JSON string below
json = "{}"
# create an instance of LoginDTO from a JSON string
login_dto_instance = LoginDTO.from_json(json)
# print the JSON string representation of the object
print(LoginDTO.to_json())

# convert the object into a dict
login_dto_dict = login_dto_instance.to_dict()
# create an instance of LoginDTO from a dict
login_dto_from_dict = LoginDTO.from_dict(login_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


