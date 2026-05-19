# CreateUserRequest

Admin: create a new user.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**full_name** | **str** |  | 
**email** | **str** |  | 
**password** | **str** |  | 
**role** | **str** |  | [optional] [default to 'viewer']
**organisation_id** | **str** |  | [optional] 

## Example

```python
from sensecore.models.create_user_request import CreateUserRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateUserRequest from a JSON string
create_user_request_instance = CreateUserRequest.from_json(json)
# print the JSON string representation of the object
print(CreateUserRequest.to_json())

# convert the object into a dict
create_user_request_dict = create_user_request_instance.to_dict()
# create an instance of CreateUserRequest from a dict
create_user_request_from_dict = CreateUserRequest.from_dict(create_user_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


