# GenreDTO

Genre including its sub-genres.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | 
**name** | **str** |  | 

## Example

```python
from songtradr_api_client_python.models.genre_dto import GenreDTO

# TODO update the JSON string below
json = "{}"
# create an instance of GenreDTO from a JSON string
genre_dto_instance = GenreDTO.from_json(json)
# print the JSON string representation of the object
print(GenreDTO.to_json())

# convert the object into a dict
genre_dto_dict = genre_dto_instance.to_dict()
# create an instance of GenreDTO from a dict
genre_dto_form_dict = genre_dto.from_dict(genre_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


