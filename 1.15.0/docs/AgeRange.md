# AgeRange


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**low** | **int** |  | [optional] 
**high** | **int** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.age_range import AgeRange

# TODO update the JSON string below
json = "{}"
# create an instance of AgeRange from a JSON string
age_range_instance = AgeRange.from_json(json)
# print the JSON string representation of the object
print AgeRange.to_json()

# convert the object into a dict
age_range_dict = age_range_instance.to_dict()
# create an instance of AgeRange from a dict
age_range_form_dict = age_range.from_dict(age_range_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


