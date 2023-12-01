# FaceDetection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timestamp** | **int** |  | [optional] 
**face** | [**FaceDetail**](FaceDetail.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.face_detection import FaceDetection

# TODO update the JSON string below
json = "{}"
# create an instance of FaceDetection from a JSON string
face_detection_instance = FaceDetection.from_json(json)
# print the JSON string representation of the object
print FaceDetection.to_json()

# convert the object into a dict
face_detection_dict = face_detection_instance.to_dict()
# create an instance of FaceDetection from a dict
face_detection_form_dict = face_detection.from_dict(face_detection_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


