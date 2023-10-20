# FaceOccluded


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **bool** |  | [optional] 
**confidence** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.face_occluded import FaceOccluded

# TODO update the JSON string below
json = "{}"
# create an instance of FaceOccluded from a JSON string
face_occluded_instance = FaceOccluded.from_json(json)
# print the JSON string representation of the object
print FaceOccluded.to_json()

# convert the object into a dict
face_occluded_dict = face_occluded_instance.to_dict()
# create an instance of FaceOccluded from a dict
face_occluded_form_dict = face_occluded.from_dict(face_occluded_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


