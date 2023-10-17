# Landmark


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**x** | **float** |  | [optional] 
**y** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.landmark import Landmark

# TODO update the JSON string below
json = "{}"
# create an instance of Landmark from a JSON string
landmark_instance = Landmark.from_json(json)
# print the JSON string representation of the object
print Landmark.to_json()

# convert the object into a dict
landmark_dict = landmark_instance.to_dict()
# create an instance of Landmark from a dict
landmark_form_dict = landmark.from_dict(landmark_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


