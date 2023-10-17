# Sunglasses


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **bool** |  | [optional] 
**confidence** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.sunglasses import Sunglasses

# TODO update the JSON string below
json = "{}"
# create an instance of Sunglasses from a JSON string
sunglasses_instance = Sunglasses.from_json(json)
# print the JSON string representation of the object
print Sunglasses.to_json()

# convert the object into a dict
sunglasses_dict = sunglasses_instance.to_dict()
# create an instance of Sunglasses from a dict
sunglasses_form_dict = sunglasses.from_dict(sunglasses_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


