# AnomalyLayer

Anomaly detection output

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**anomaly_detected** | **bool** |  | 
**anomaly_score** | **float** |  | 
**anomaly_periods** | **List[int]** |  | 
**anomaly_description** | **str** |  | 

## Example

```python
from sensecore.models.anomaly_layer import AnomalyLayer

# TODO update the JSON string below
json = "{}"
# create an instance of AnomalyLayer from a JSON string
anomaly_layer_instance = AnomalyLayer.from_json(json)
# print the JSON string representation of the object
print(AnomalyLayer.to_json())

# convert the object into a dict
anomaly_layer_dict = anomaly_layer_instance.to_dict()
# create an instance of AnomalyLayer from a dict
anomaly_layer_from_dict = AnomalyLayer.from_dict(anomaly_layer_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


