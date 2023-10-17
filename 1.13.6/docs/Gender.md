# Gender


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **str** |  | [optional] 
**confidence** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.gender import Gender

# TODO update the JSON string below
json = "{}"
# create an instance of Gender from a JSON string
gender_instance = Gender.from_json(json)
# print the JSON string representation of the object
print Gender.to_json()

# convert the object into a dict
gender_dict = gender_instance.to_dict()
# create an instance of Gender from a dict
gender_form_dict = gender.from_dict(gender_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


