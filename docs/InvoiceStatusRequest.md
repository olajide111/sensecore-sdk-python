# InvoiceStatusRequest

Admin: update invoice status.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**invoice_id** | **str** |  | 
**status** | **str** |  | 
**amount_paid** | **float** |  | [optional] 

## Example

```python
from sensecore.models.invoice_status_request import InvoiceStatusRequest

# TODO update the JSON string below
json = "{}"
# create an instance of InvoiceStatusRequest from a JSON string
invoice_status_request_instance = InvoiceStatusRequest.from_json(json)
# print the JSON string representation of the object
print(InvoiceStatusRequest.to_json())

# convert the object into a dict
invoice_status_request_dict = invoice_status_request_instance.to_dict()
# create an instance of InvoiceStatusRequest from a dict
invoice_status_request_from_dict = InvoiceStatusRequest.from_dict(invoice_status_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


