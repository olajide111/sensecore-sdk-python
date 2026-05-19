# PersonaRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**persona** | **str** |  | 
**seed_demo** | **bool** |  | [optional] [default to True]

## Example

```python
from sensecore.models.persona_request import PersonaRequest

# TODO update the JSON string below
json = "{}"
# create an instance of PersonaRequest from a JSON string
persona_request_instance = PersonaRequest.from_json(json)
# print the JSON string representation of the object
print(PersonaRequest.to_json())

# convert the object into a dict
persona_request_dict = persona_request_instance.to_dict()
# create an instance of PersonaRequest from a dict
persona_request_from_dict = PersonaRequest.from_dict(persona_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


