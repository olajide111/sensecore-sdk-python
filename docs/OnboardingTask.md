# OnboardingTask


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**title** | **str** |  | 
**description** | **str** |  | 
**complete** | **bool** |  | 
**action_url** | **str** |  | 

## Example

```python
from sensecore.models.onboarding_task import OnboardingTask

# TODO update the JSON string below
json = "{}"
# create an instance of OnboardingTask from a JSON string
onboarding_task_instance = OnboardingTask.from_json(json)
# print the JSON string representation of the object
print(OnboardingTask.to_json())

# convert the object into a dict
onboarding_task_dict = onboarding_task_instance.to_dict()
# create an instance of OnboardingTask from a dict
onboarding_task_from_dict = OnboardingTask.from_dict(onboarding_task_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


