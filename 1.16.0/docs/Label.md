# Label


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** |  | [optional] 
**confidence** | **float** |  | [optional] 
**instances** | [**List[Instance]**](Instance.md) |  | [optional] 
**parents** | [**List[Parent]**](Parent.md) |  | [optional] 
**aliases** | [**List[LabelAlias]**](LabelAlias.md) |  | [optional] 
**categories** | [**List[LabelCategory]**](LabelCategory.md) |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.label import Label

# TODO update the JSON string below
json = "{}"
# create an instance of Label from a JSON string
label_instance = Label.from_json(json)
# print the JSON string representation of the object
print Label.to_json()

# convert the object into a dict
label_dict = label_instance.to_dict()
# create an instance of Label from a dict
label_form_dict = label.from_dict(label_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


