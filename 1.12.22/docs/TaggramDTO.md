# TaggramDTO

A TaggramDTO for recordings.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timeseries** | **List[float]** | Values represent the strength of presence of the corresponding category, tag or genre. | 
**category_name** | **str** |  | 
**tag_name** | **str** |  | [optional] 
**genre_name** | **str** |  | [optional] 
**scale** | **List[int]** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.taggram_dto import TaggramDTO

# TODO update the JSON string below
json = "{}"
# create an instance of TaggramDTO from a JSON string
taggram_dto_instance = TaggramDTO.from_json(json)
# print the JSON string representation of the object
print TaggramDTO.to_json()

# convert the object into a dict
taggram_dto_dict = taggram_dto_instance.to_dict()
# create an instance of TaggramDTO from a dict
taggram_dto_form_dict = taggram_dto.from_dict(taggram_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


