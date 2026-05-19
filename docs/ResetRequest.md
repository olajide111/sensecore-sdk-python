# ResetRequest

Password reset - step 2: set new password.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**token** | **str** |  | 
**new_password** | **str** |  | 

## Example

```python
from sensecore.models.reset_request import ResetRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ResetRequest from a JSON string
reset_request_instance = ResetRequest.from_json(json)
# print the JSON string representation of the object
print(ResetRequest.to_json())

# convert the object into a dict
reset_request_dict = reset_request_instance.to_dict()
# create an instance of ResetRequest from a dict
reset_request_from_dict = ResetRequest.from_dict(reset_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


