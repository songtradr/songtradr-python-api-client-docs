# EyeDirection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**yaw** | **float** |  | [optional] 
**pitch** | **float** |  | [optional] 
**confidence** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.eye_direction import EyeDirection

# TODO update the JSON string below
json = "{}"
# create an instance of EyeDirection from a JSON string
eye_direction_instance = EyeDirection.from_json(json)
# print the JSON string representation of the object
print EyeDirection.to_json()

# convert the object into a dict
eye_direction_dict = eye_direction_instance.to_dict()
# create an instance of EyeDirection from a dict
eye_direction_form_dict = eye_direction.from_dict(eye_direction_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


