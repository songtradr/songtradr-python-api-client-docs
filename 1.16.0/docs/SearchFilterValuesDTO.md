# SearchFilterValuesDTO

Categories of musical features that can be used as search filters.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**primary_mood_cluster** | **List[str]** |  | 
**secondary_mood_cluster** | **List[str]** |  | 
**tertiary_mood_cluster** | **List[str]** |  | 
**valence** | **List[str]** |  | 
**arousal** | **List[str]** |  | 
**pleasantness** | **List[str]** |  | 
**engagement** | **List[str]** |  | 
**vocals** | **List[str]** |  | 
**dominant_instrument** | **List[str]** |  | 
**secondary_instrument** | **List[str]** |  | 
**tertiary_instrument** | **List[str]** |  | 
**energy** | **List[str]** |  | 
**sound_generation** | **List[str]** |  | 
**tempo** | **List[str]** |  | 
**scale** | **List[str]** |  | 
**key** | **List[str]** |  | 
**rhythm** | **List[str]** |  | 
**primary_sound_character** | **List[str]** |  | 
**timbre** | **List[str]** |  | 
**roughness** | **List[str]** |  | 
**tonality** | **List[str]** |  | 
**harmony** | **List[str]** |  | 
**texture** | **List[str]** |  | 
**groovyness** | **List[str]** |  | 
**space** | **List[str]** |  | 
**production_rating** | **List[str]** |  | 
**performance_rating** | **List[str]** |  | 
**song_rating** | **List[str]** |  | 
**audience_age** | **List[str]** |  | 
**secondary_audience_age** | **List[str]** |  | 
**tertiary_audience_age** | **List[str]** |  | 
**audience_gender** | **List[str]** |  | 
**audience_region** | **List[str]** |  | 
**secondary_audience_region** | **List[str]** |  | 
**tertiary_audience_region** | **List[str]** |  | 
**origin_decade** | **List[str]** |  | 
**origin_region** | **List[str]** |  | 
**language_of_performance** | **List[str]** |  | 
**curateability** | **List[str]** |  | 
**use_case** | **List[str]** |  | 
**channel_suitability** | **List[str]** |  | 

## Example

```python
from songtradr_api_client_python.models.search_filter_values_dto import SearchFilterValuesDTO

# TODO update the JSON string below
json = "{}"
# create an instance of SearchFilterValuesDTO from a JSON string
search_filter_values_dto_instance = SearchFilterValuesDTO.from_json(json)
# print the JSON string representation of the object
print SearchFilterValuesDTO.to_json()

# convert the object into a dict
search_filter_values_dto_dict = search_filter_values_dto_instance.to_dict()
# create an instance of SearchFilterValuesDTO from a dict
search_filter_values_dto_form_dict = search_filter_values_dto.from_dict(search_filter_values_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


