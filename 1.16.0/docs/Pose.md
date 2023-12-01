# Pose


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**roll** | **float** |  | [optional] 
**yaw** | **float** |  | [optional] 
**pitch** | **float** |  | [optional] 

## Example

```python
from songtradr_api_client_python.models.pose import Pose

# TODO update the JSON string below
json = "{}"
# create an instance of Pose from a JSON string
pose_instance = Pose.from_json(json)
# print the JSON string representation of the object
print Pose.to_json()

# convert the object into a dict
pose_dict = pose_instance.to_dict()
# create an instance of Pose from a dict
pose_form_dict = pose.from_dict(pose_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


