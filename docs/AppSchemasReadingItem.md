# AppSchemasReadingItem


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**timestamp** | **datetime** |  | 
**kwh** | **float** |  | 

## Example

```python
from sensecore.models.app_schemas_reading_item import AppSchemasReadingItem

# TODO update the JSON string below
json = "{}"
# create an instance of AppSchemasReadingItem from a JSON string
app_schemas_reading_item_instance = AppSchemasReadingItem.from_json(json)
# print the JSON string representation of the object
print(AppSchemasReadingItem.to_json())

# convert the object into a dict
app_schemas_reading_item_dict = app_schemas_reading_item_instance.to_dict()
# create an instance of AppSchemasReadingItem from a dict
app_schemas_reading_item_from_dict = AppSchemasReadingItem.from_dict(app_schemas_reading_item_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


