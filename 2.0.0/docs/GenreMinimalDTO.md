# GenreMinimalDTO

Genre in its minimal form.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**genre_name** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.genre_minimal_dto import GenreMinimalDTO

# TODO update the JSON string below
json = "{}"
# create an instance of GenreMinimalDTO from a JSON string
genre_minimal_dto_instance = GenreMinimalDTO.from_json(json)
# print the JSON string representation of the object
print(GenreMinimalDTO.to_json())

# convert the object into a dict
genre_minimal_dto_dict = genre_minimal_dto_instance.to_dict()
# create an instance of GenreMinimalDTO from a dict
genre_minimal_dto_form_dict = genre_minimal_dto.from_dict(genre_minimal_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


