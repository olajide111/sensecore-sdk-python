# CreateInvoiceRequest

Admin: generate a new invoice for an organisation.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**org_id** | **str** |  | 
**amount** | **float** |  | [optional] [default to 0]
**plan** | **str** |  | [optional] [default to 'custom']
**billing_cycle** | **str** |  | [optional] [default to 'monthly']
**description** | **str** |  | [optional] [default to 'SenseCore AI Platform']
**client_address** | **str** |  | [optional] 
**client_phone** | **str** |  | [optional] 

## Example

```python
from sensecore.models.create_invoice_request import CreateInvoiceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of CreateInvoiceRequest from a JSON string
create_invoice_request_instance = CreateInvoiceRequest.from_json(json)
# print the JSON string representation of the object
print(CreateInvoiceRequest.to_json())

# convert the object into a dict
create_invoice_request_dict = create_invoice_request_instance.to_dict()
# create an instance of CreateInvoiceRequest from a dict
create_invoice_request_from_dict = CreateInvoiceRequest.from_dict(create_invoice_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


