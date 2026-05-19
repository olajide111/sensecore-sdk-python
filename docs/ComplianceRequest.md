# ComplianceRequest


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**meter_id** | **str** |  | [optional] 
**org_id** | **str** |  | [optional] 
**period** | **str** |  | [optional] [default to 'annual']
**year** | **int** |  | [optional] 
**readings** | **List[object]** |  | [optional] 
**revenue_gbp** | **float** |  | [optional] 
**floor_area_m2** | **float** |  | [optional] 
**fte_count** | **int** |  | [optional] 

## Example

```python
from sensecore.models.compliance_request import ComplianceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of ComplianceRequest from a JSON string
compliance_request_instance = ComplianceRequest.from_json(json)
# print the JSON string representation of the object
print(ComplianceRequest.to_json())

# convert the object into a dict
compliance_request_dict = compliance_request_instance.to_dict()
# create an instance of ComplianceRequest from a dict
compliance_request_from_dict = ComplianceRequest.from_dict(compliance_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


