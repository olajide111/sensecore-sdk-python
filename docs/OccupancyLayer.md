# OccupancyLayer

Inferred building occupancy from consumption patterns

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**occupancy_rate** | **float** |  | 
**occupied_periods** | **List[int]** |  | 
**peak_occupancy_hour** | **int** |  | 
**pattern_type** | **str** |  | 

## Example

```python
from sensecore.models.occupancy_layer import OccupancyLayer

# TODO update the JSON string below
json = "{}"
# create an instance of OccupancyLayer from a JSON string
occupancy_layer_instance = OccupancyLayer.from_json(json)
# print the JSON string representation of the object
print(OccupancyLayer.to_json())

# convert the object into a dict
occupancy_layer_dict = occupancy_layer_instance.to_dict()
# create an instance of OccupancyLayer from a dict
occupancy_layer_from_dict = OccupancyLayer.from_dict(occupancy_layer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


