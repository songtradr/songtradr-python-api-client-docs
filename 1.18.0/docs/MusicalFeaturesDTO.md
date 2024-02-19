# MusicalFeaturesDTO

AI generated musical features of a recording.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**space** | **str** | Search for space | [optional] 
**secondary_mood_cluster** | **str** | Search for a language of the lyrics | [optional] 
**secondary_mood_cluster_affinity** | **float** |  | [optional] 
**tertiary_mood_cluster** | **str** | Search for a language of the lyrics | [optional] 
**tertiary_mood_cluster_affinity** | **float** |  | [optional] 
**vocals_affinity** | **float** |  | [optional] 
**dominant_instrument_affinity** | **float** |  | [optional] 
**secondary_instrument** | **str** | Search for a dominant instrument | [optional] 
**secondary_instrument_affinity** | **float** |  | [optional] 
**tertiary_instrument** | **str** | Search for a dominant instrument | [optional] 
**tertiary_instrument_affinity** | **float** |  | [optional] 
**sound_generation_affinity** | **float** |  | [optional] 
**rhythm_affinity** | **float** |  | [optional] 
**primary_sound_character_affinity** | **float** |  | [optional] 
**tonality_affinity** | **float** |  | [optional] 
**bpm** | **float** |  | [optional] 
**production_rating** | **str** |  | [optional] 
**production_rating_affinity** | **float** |  | [optional] 
**performance_rating** | **str** |  | [optional] 
**performance_rating_affinity** | **float** |  | [optional] 
**song_rating** | **str** |  | [optional] 
**song_rating_affinity** | **float** |  | [optional] 
**primary_mood_cluster_affinity** | **float** |  | [optional] 
**audience_age** | **str** |  | [optional] 
**audience_age_affinity** | **float** |  | [optional] 
**secondary_audience_age** | **str** |  | [optional] 
**secondary_audience_age_affinity** | **float** |  | [optional] 
**tertiary_audience_age** | **str** |  | [optional] 
**tertiary_audience_age_affinity** | **float** |  | [optional] 
**audience_gender** | **str** |  | [optional] 
**audience_gender_affinity** | **float** |  | [optional] 
**audience_region_affinity** | **float** |  | [optional] 
**secondary_audience_region** | **str** |  | [optional] 
**secondary_audience_region_affinity** | **float** |  | [optional] 
**tertiary_audience_region** | **str** |  | [optional] 
**tertiary_audience_region_affinity** | **float** |  | [optional] 
**origin_region** | **str** |  | [optional] 
**origin_region_affinity** | **float** |  | [optional] 
**origin_decade_affinity** | **float** |  | [optional] 
**language_of_performance_affinity** | **float** |  | [optional] 
**curateability_affinity** | **float** |  | [optional] 
**use_case_affinity** | **float** |  | [optional] 
**industry_suitability** | **str** | Search for Industry suitability | [optional] 
**industry_suitability_affinity** | **float** |  | [optional] 
**audience_region** | **str** |  | [optional] 
**arousal** | **str** | Search for an arousal | [optional] 
**dominant_instrument** | **str** | Search for a dominant instrument | [optional] 
**energy** | **str** | Search for energy | [optional] 
**engagement** | **str** | Search for an engagement | [optional] 
**groovyness** | **str** | Search for groovyness | [optional] 
**harmony** | **str** | Search for a degree of harmoniousness | [optional] 
**pleasantness** | **str** | Search for pleasantness | [optional] 
**primary_mood_cluster** | **str** | Search for a language of the lyrics | [optional] 
**primary_sound_character** | **str** | Search for a sound character | [optional] 
**rhythm** | **str** | Search for rhythm | [optional] 
**roughness** | **str** | Search for roughness | [optional] 
**scale** | **str** | Search for a tonal scale | [optional] 
**key** | **str** | Search for a harmonic key | [optional] 
**sound_generation** | **str** | Search for type of sound generation | [optional] 
**tempo** | **str** | Search for tempo | [optional] 
**texture** | **str** | Search for texture | [optional] 
**timbre** | **str** | Search for timbre | [optional] 
**tonality** | **str** | Search for tonality | [optional] 
**valence** | **str** | Search for a valence | [optional] 
**vocals** | **str** | Search for a vocal gender or instrumental songs | [optional] 
**origin_decade** | **str** | Search for origin decade | [optional] 
**curateability** | **str** | Search for curatebility | [optional] 
**use_case** | **str** | Search for use case | [optional] 
**channel_suitability** | **str** | Search for social media suitability | [optional] 
**loudness** | **str** | Search for loudness | [optional] 
**language_of_performance** | **str** |  | [optional] 
**valence_affinity** | **float** |  | [optional] 
**arousal_affinity** | **float** |  | [optional] 
**pleasantness_affinity** | **float** |  | [optional] 
**engagement_affinity** | **float** |  | [optional] 
**energy_affinity** | **float** |  | [optional] 
**tempo_affinity** | **float** |  | [optional] 
**scale_affinity** | **float** |  | [optional] 
**timbre_affinity** | **float** |  | [optional] 
**roughness_affinity** | **float** |  | [optional] 
**harmony_affinity** | **float** |  | [optional] 
**texture_affinity** | **float** |  | [optional] 
**groovyness_affinity** | **float** |  | [optional] 
**space_affinity** | **float** |  | [optional] 
**loudness_affinity** | **float** |  | [optional] 
**key_affinity** | **float** |  | [optional] 
**channel_suitability_affinity** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.musical_features_dto import MusicalFeaturesDTO

# TODO update the JSON string below
json = "{}"
# create an instance of MusicalFeaturesDTO from a JSON string
musical_features_dto_instance = MusicalFeaturesDTO.from_json(json)
# print the JSON string representation of the object
print MusicalFeaturesDTO.to_json()

# convert the object into a dict
musical_features_dto_dict = musical_features_dto_instance.to_dict()
# create an instance of MusicalFeaturesDTO from a dict
musical_features_dto_form_dict = musical_features_dto.from_dict(musical_features_dto_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


