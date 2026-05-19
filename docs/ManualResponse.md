# ManualResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | 
**timestamp** | **str** |  | 
**kwh** | **float** |  | 
**status** | **str** |  | 
**message** | **str** |  | 

## Example

```python
from sensecore.models.manual_response import ManualResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ManualResponse from a JSON string
manual_response_instance = ManualResponse.from_json(json)
# print the JSON string representation of the object
print(ManualResponse.to_json())

# convert the object into a dict
manual_response_dict = manual_response_instance.to_dict()
# create an instance of ManualResponse from a dict
manual_response_from_dict = ManualResponse.from_dict(manual_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


