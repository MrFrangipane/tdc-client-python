# Expense


## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **str** |  | 
**project** | [**Project**](Project.md) |  | 
**caption** | **str** |  | 
**amount** | **float** |  | 
**date_** | **date** |  | 
**needs_refund** | **bool** |  | [optional] [default to False]
**refunded** | **bool** |  | [optional] 
**date_refund** | **date** |  | [optional] 

## Example

```python
from tdc_api_client.models.expense import Expense

# TODO update the JSON string below
json = "{}"
# create an instance of Expense from a JSON string
expense_instance = Expense.from_json(json)
# print the JSON string representation of the object
print Expense.to_json()

# convert the object into a dict
expense_dict = expense_instance.to_dict()
# create an instance of Expense from a dict
expense_form_dict = expense.from_dict(expense_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


