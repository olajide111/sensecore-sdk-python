# LeadCaptureRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**conversation_id** | **str** |  | 
**email** | **str** |  | 
**name** | **str** |  | [optional] [default to '']
**organisation** | **str** |  | [optional] [default to '']
**phone** | **str** |  | [optional] [default to '']
**sector** | **str** |  | [optional] [default to '']
**source** | **str** |  | [optional] [default to 'marketing']

## Example

```python
from sensecore.models.lead_capture_request import LeadCaptureRequest

# TODO update the JSON string below
json = "{}"
# create an instance of LeadCaptureRequest from a JSON string
lead_capture_request_instance = LeadCaptureRequest.from_json(json)
# print the JSON string representation of the object
print(LeadCaptureRequest.to_json())

# convert the object into a dict
lead_capture_request_dict = lead_capture_request_instance.to_dict()
# create an instance of LeadCaptureRequest from a dict
lead_capture_request_from_dict = LeadCaptureRequest.from_dict(lead_capture_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


