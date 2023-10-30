# Instance


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bounding_box** | [**BoundingBox**](BoundingBox.md) |  | [optional] 
**confidence** | **float** |  | [optional] 
**dominant_colors** | [**List[DominantColor]**](DominantColor.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.instance import Instance

# TODO update the JSON string below
json = "{}"
# create an instance of Instance from a JSON string
instance_instance = Instance.from_json(json)
# print the JSON string representation of the object
print Instance.to_json()

# convert the object into a dict
instance_dict = instance_instance.to_dict()
# create an instance of Instance from a dict
instance_form_dict = instance.from_dict(instance_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


