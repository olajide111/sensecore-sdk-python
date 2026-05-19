# ForgotRequest

Password reset - step 1: request reset link.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**email** | **str** |  | 

## Example

```python
from sensecore.models.forgot_request import ForgotRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ForgotRequest from a JSON string
forgot_request_instance = ForgotRequest.from_json(json)
# print the JSON string representation of the object
print(ForgotRequest.to_json())

# convert the object into a dict
forgot_request_dict = forgot_request_instance.to_dict()
# create an instance of ForgotRequest from a dict
forgot_request_from_dict = ForgotRequest.from_dict(forgot_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


