# LabelDetection


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timestamp** | **int** |  | [optional] 
**label** | [**Label**](Label.md) |  | [optional] 
**start_timestamp_millis** | **int** |  | [optional] 
**end_timestamp_millis** | **int** |  | [optional] 
**duration_millis** | **int** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.label_detection import LabelDetection

# TODO update the JSON string below
json = "{}"
# create an instance of LabelDetection from a JSON string
label_detection_instance = LabelDetection.from_json(json)
# print the JSON string representation of the object
print LabelDetection.to_json()

# convert the object into a dict
label_detection_dict = label_detection_instance.to_dict()
# create an instance of LabelDetection from a dict
label_detection_form_dict = label_detection.from_dict(label_detection_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


