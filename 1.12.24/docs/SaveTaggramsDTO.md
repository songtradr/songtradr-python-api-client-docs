# SaveTaggramsDTO

Timeseries of tags.

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timestamps** | **List[float]** |  | [optional] 
**level1_genre** | **Dict[str, List[float]]** |  | [optional] 
**level2_genre** | **Dict[str, List[float]]** |  | [optional] 
**song_rating** | **Dict[str, List[float]]** |  | [optional] 
**performance_rating** | **Dict[str, List[float]]** |  | [optional] 
**production_rating** | **Dict[str, List[float]]** |  | [optional] 
**mood_cluster** | **Dict[str, List[float]]** |  | [optional] 
**vocals** | **Dict[str, List[float]]** |  | [optional] 
**dominant_instrument** | **Dict[str, List[float]]** |  | [optional] 
**sound_generation** | **Dict[str, List[float]]** |  | [optional] 
**rhythm** | **Dict[str, List[float]]** |  | [optional] 
**tonality** | **Dict[str, List[float]]** |  | [optional] 
**audience_age** | **Dict[str, List[float]]** |  | [optional] 
**audience_gender** | **Dict[str, List[float]]** |  | [optional] 
**audience_region** | **Dict[str, List[float]]** |  | [optional] 
**origin_region** | **Dict[str, List[float]]** |  | [optional] 
**origin_decade** | **Dict[str, List[float]]** |  | [optional] 
**language_of_performance** | **Dict[str, List[float]]** |  | [optional] 
**arousal** | **Dict[str, List[float]]** |  | [optional] 
**valence** | **Dict[str, List[float]]** |  | [optional] 
**pleasantness** | **Dict[str, List[float]]** |  | [optional] 
**engagement** | **Dict[str, List[float]]** |  | [optional] 
**energy** | **Dict[str, List[float]]** |  | [optional] 
**timbre** | **Dict[str, List[float]]** |  | [optional] 
**roughness** | **Dict[str, List[float]]** |  | [optional] 
**harmony** | **Dict[str, List[float]]** |  | [optional] 
**texture** | **Dict[str, List[float]]** |  | [optional] 
**groovyness** | **Dict[str, List[float]]** |  | [optional] 
**space** | **Dict[str, List[float]]** |  | [optional] 
**curateability** | **Dict[str, List[float]]** |  | [optional] 
**use_case** | **Dict[str, List[float]]** |  | [optional] 
**social_media** | **Dict[str, List[float]]** |  | [optional] 
**industry_suitability** | **Dict[str, List[float]]** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.save_taggrams_dto import SaveTaggramsDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SaveTaggramsDTO from a JSON string
save_taggrams_dto_instance = SaveTaggramsDTO.from_json(json)
# print the JSON string representation of the object
print SaveTaggramsDTO.to_json()

# convert the object into a dict
save_taggrams_dto_dict = save_taggrams_dto_instance.to_dict()
# create an instance of SaveTaggramsDTO from a dict
save_taggrams_dto_form_dict = save_taggrams_dto.from_dict(save_taggrams_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


