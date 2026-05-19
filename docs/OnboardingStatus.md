# OnboardingStatus


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**persona** | **str** |  | 
**dismissed_at** | **str** |  | 
**completed_at** | **str** |  | 
**portfolio_type** | **str** |  | 
**tour_completed_at** | **str** |  | 
**tasks** | [**List[OnboardingTask]**](OnboardingTask.md) |  | 
**progress** | **int** |  | 
**show_celebration** | **bool** |  | 

## Example

```python
from sensecore.models.onboarding_status import OnboardingStatus

# TODO update the JSON string below
json = "{}"
# create an instance of OnboardingStatus from a JSON string
onboarding_status_instance = OnboardingStatus.from_json(json)
# print the JSON string representation of the object
print(OnboardingStatus.to_json())

# convert the object into a dict
onboarding_status_dict = onboarding_status_instance.to_dict()
# create an instance of OnboardingStatus from a dict
onboarding_status_from_dict = OnboardingStatus.from_dict(onboarding_status_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


