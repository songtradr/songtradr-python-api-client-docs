# Emotion


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**type** | **str** |  | [optional] 
**confidence** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.emotion import Emotion

# TODO update the JSON string below
json = "{}"
# create an instance of Emotion from a JSON string
emotion_instance = Emotion.from_json(json)
# print the JSON string representation of the object
print Emotion.to_json()

# convert the object into a dict
emotion_dict = emotion_instance.to_dict()
# create an instance of Emotion from a dict
emotion_form_dict = emotion.from_dict(emotion_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


