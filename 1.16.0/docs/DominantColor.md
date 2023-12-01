# DominantColor


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**red** | **int** |  | [optional] 
**blue** | **int** |  | [optional] 
**green** | **int** |  | [optional] 
**hex_code** | **str** |  | [optional] 
**simplified_color** | **str** |  | [optional] 
**pixel_percent** | **float** |  | [optional] 
**csscolor** | **str** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.dominant_color import DominantColor

# TODO update the JSON string below
json = "{}"
# create an instance of DominantColor from a JSON string
dominant_color_instance = DominantColor.from_json(json)
# print the JSON string representation of the object
print DominantColor.to_json()

# convert the object into a dict
dominant_color_dict = dominant_color_instance.to_dict()
# create an instance of DominantColor from a dict
dominant_color_form_dict = dominant_color.from_dict(dominant_color_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


