# CreateAPIKeyRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **str** | Display label, e.g. &#39;Production ingest&#39; or &#39;Reporting dashboard&#39; | 

## Example

```python
from sensecore.models.create_api_key_request import CreateAPIKeyRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateAPIKeyRequest from a JSON string
create_api_key_request_instance = CreateAPIKeyRequest.from_json(json)
# print the JSON string representation of the object
print(CreateAPIKeyRequest.to_json())

# convert the object into a dict
create_api_key_request_dict = create_api_key_request_instance.to_dict()
# create an instance of CreateAPIKeyRequest from a dict
create_api_key_request_from_dict = CreateAPIKeyRequest.from_dict(create_api_key_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


