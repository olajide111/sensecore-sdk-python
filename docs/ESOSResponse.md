# ESOSResponse


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**report_type** | **str** |  | [optional] [default to 'ESOS Phase 4']
**organisation** | **str** |  | 
**period** | **str** |  | 
**year** | **int** |  | 
**generated_at** | **str** |  | 
**total_energy_kwh** | **float** |  | 
**significant_energy_consumption** | **List[object]** |  | 
**energy_audits** | **List[object]** |  | 
**recommendations** | **List[object]** |  | 
**compliance_route** | **str** |  | 
**lead_assessor_required** | **bool** |  | [optional] [default to True]
**status** | **str** |  | [optional] [default to 'evidence_pack']

## Example

```python
from sensecore.models.esos_response import ESOSResponse

# TODO update the JSON string below
json = "{}"
# create an instance of ESOSResponse from a JSON string
esos_response_instance = ESOSResponse.from_json(json)
# print the JSON string representation of the object
print(ESOSResponse.to_json())

# convert the object into a dict
esos_response_dict = esos_response_instance.to_dict()
# create an instance of ESOSResponse from a dict
esos_response_from_dict = ESOSResponse.from_dict(esos_response_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


