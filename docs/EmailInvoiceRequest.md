# EmailInvoiceRequest

Request body for emailing a single invoice.

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**recipient_email** | **str** |  | 
**cc_emails** | **str** |  | [optional] 
**message** | **str** |  | [optional] 
**copy_to_sender** | **bool** |  | [optional] [default to False]

## Example

```python
from sensecore.models.email_invoice_request import EmailInvoiceRequest

# TODO update the JSON string below
json = "{}"
# create an instance of EmailInvoiceRequest from a JSON string
email_invoice_request_instance = EmailInvoiceRequest.from_json(json)
# print the JSON string representation of the object
print(EmailInvoiceRequest.to_json())

# convert the object into a dict
email_invoice_request_dict = email_invoice_request_instance.to_dict()
# create an instance of EmailInvoiceRequest from a dict
email_invoice_request_from_dict = EmailInvoiceRequest.from_dict(email_invoice_request_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


