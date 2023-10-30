# ImageQuality


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**brightness** | **float** |  | [optional] 
**sharpness** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.image_quality import ImageQuality

# TODO update the JSON string below
json = "{}"
# create an instance of ImageQuality from a JSON string
image_quality_instance = ImageQuality.from_json(json)
# print the JSON string representation of the object
print ImageQuality.to_json()

# convert the object into a dict
image_quality_dict = image_quality_instance.to_dict()
# create an instance of ImageQuality from a dict
image_quality_form_dict = image_quality.from_dict(image_quality_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


