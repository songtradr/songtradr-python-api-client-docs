# FaceDetail


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bounding_box** | [**BoundingBox**](BoundingBox.md) |  | [optional] 
**age_range** | [**AgeRange**](AgeRange.md) |  | [optional] 
**smile** | [**Smile**](Smile.md) |  | [optional] 
**eyeglasses** | [**Eyeglasses**](Eyeglasses.md) |  | [optional] 
**sunglasses** | [**Sunglasses**](Sunglasses.md) |  | [optional] 
**gender** | [**Gender**](Gender.md) |  | [optional] 
**beard** | [**Beard**](Beard.md) |  | [optional] 
**mustache** | [**Mustache**](Mustache.md) |  | [optional] 
**eyes_open** | [**EyeOpen**](EyeOpen.md) |  | [optional] 
**mouth_open** | [**MouthOpen**](MouthOpen.md) |  | [optional] 
**emotions** | [**List[Emotion]**](Emotion.md) |  | [optional] 
**landmarks** | [**List[Landmark]**](Landmark.md) |  | [optional] 
**pose** | [**Pose**](Pose.md) |  | [optional] 
**quality** | [**ImageQuality**](ImageQuality.md) |  | [optional] 
**confidence** | **float** |  | [optional] 
**face_occluded** | [**FaceOccluded**](FaceOccluded.md) |  | [optional] 
**eye_direction** | [**EyeDirection**](EyeDirection.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.face_detail import FaceDetail

# TODO update the JSON string below
json = "{}"
# create an instance of FaceDetail from a JSON string
face_detail_instance = FaceDetail.from_json(json)
# print the JSON string representation of the object
print FaceDetail.to_json()

# convert the object into a dict
face_detail_dict = face_detail_instance.to_dict()
# create an instance of FaceDetail from a dict
face_detail_form_dict = face_detail.from_dict(face_detail_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


