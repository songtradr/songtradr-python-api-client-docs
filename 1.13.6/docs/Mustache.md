# Mustache


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**value** | **bool** |  | [optional] 
**confidence** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.mustache import Mustache

# TODO update the JSON string below
json = "{}"
# create an instance of Mustache from a JSON string
mustache_instance = Mustache.from_json(json)
# print the JSON string representation of the object
print Mustache.to_json()

# convert the object into a dict
mustache_dict = mustache_instance.to_dict()
# create an instance of Mustache from a dict
mustache_form_dict = mustache.from_dict(mustache_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


