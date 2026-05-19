# AppRoutersReadingsPushReadingItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timestamp** | **str** |  | 
**kwh** | **float** |  | 

## Example

```python
from sensecore.models.app_routers_readings_push_reading_item import AppRoutersReadingsPushReadingItem

# TODO update the JSON string below
json = "{}"
# create an instance of AppRoutersReadingsPushReadingItem from a JSON string
app_routers_readings_push_reading_item_instance = AppRoutersReadingsPushReadingItem.from_json(json)
# print the JSON string representation of the object
print(AppRoutersReadingsPushReadingItem.to_json())

# convert the object into a dict
app_routers_readings_push_reading_item_dict = app_routers_readings_push_reading_item_instance.to_dict()
# create an instance of AppRoutersReadingsPushReadingItem from a dict
app_routers_readings_push_reading_item_from_dict = AppRoutersReadingsPushReadingItem.from_dict(app_routers_readings_push_reading_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


