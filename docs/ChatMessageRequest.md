# ChatMessageRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**message** | **str** |  | 
**session_id** | **str** |  | 
**source** | **str** |  | [optional] [default to 'marketing']

## Example

```python
from sensecore.models.chat_message_request import ChatMessageRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ChatMessageRequest from a JSON string
chat_message_request_instance = ChatMessageRequest.from_json(json)
# print the JSON string representation of the object
print(ChatMessageRequest.to_json())

# convert the object into a dict
chat_message_request_dict = chat_message_request_instance.to_dict()
# create an instance of ChatMessageRequest from a dict
chat_message_request_from_dict = ChatMessageRequest.from_dict(chat_message_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


