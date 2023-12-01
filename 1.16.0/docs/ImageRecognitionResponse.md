# ImageRecognitionResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**labels** | [**List[Label]**](Label.md) |  | [optional] 
**faces** | [**List[FaceDetail]**](FaceDetail.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.image_recognition_response import ImageRecognitionResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ImageRecognitionResponse from a JSON string
image_recognition_response_instance = ImageRecognitionResponse.from_json(json)
# print the JSON string representation of the object
print ImageRecognitionResponse.to_json()

# convert the object into a dict
image_recognition_response_dict = image_recognition_response_instance.to_dict()
# create an instance of ImageRecognitionResponse from a dict
image_recognition_response_form_dict = image_recognition_response.from_dict(image_recognition_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


