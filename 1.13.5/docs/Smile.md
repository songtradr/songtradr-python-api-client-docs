# Smile


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **bool** |  | [optional] 
**confidence** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.smile import Smile

# TODO update the JSON string below
json = "{}"
# create an instance of Smile from a JSON string
smile_instance = Smile.from_json(json)
# print the JSON string representation of the object
print Smile.to_json()

# convert the object into a dict
smile_dict = smile_instance.to_dict()
# create an instance of Smile from a dict
smile_form_dict = smile.from_dict(smile_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


