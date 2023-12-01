# VideoRecognitionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**labels** | [**List[LabelDetection]**](LabelDetection.md) |  | [optional] 
**faces** | [**List[FaceDetection]**](FaceDetection.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.video_recognition_response import VideoRecognitionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of VideoRecognitionResponse from a JSON string
video_recognition_response_instance = VideoRecognitionResponse.from_json(json)
# print the JSON string representation of the object
print VideoRecognitionResponse.to_json()

# convert the object into a dict
video_recognition_response_dict = video_recognition_response_instance.to_dict()
# create an instance of VideoRecognitionResponse from a dict
video_recognition_response_form_dict = video_recognition_response.from_dict(video_recognition_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


