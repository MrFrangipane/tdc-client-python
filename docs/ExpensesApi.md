# tdc_api_client.ExpensesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_expenses_expense_id_get**](ExpensesApi.md#get_expenses_expense_id_get) | **GET** /expenses/{expense_id} | Get
[**get_expenses_get**](ExpensesApi.md#get_expenses_get) | **GET** /expenses/ | Get
[**get_project_expenses_project_id_expenses_get**](ExpensesApi.md#get_project_expenses_project_id_expenses_get) | **GET** /expenses/{project_id}/expenses | Get Project
[**post_expenses_post**](ExpensesApi.md#post_expenses_post) | **POST** /expenses/ | Post


# **get_expenses_expense_id_get**
> Expense get_expenses_expense_id_get(expense_id)

Get

### Example

```python
import time
import os
import tdc_api_client
from tdc_api_client.models.expense import Expense
from tdc_api_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = tdc_api_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with tdc_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = tdc_api_client.ExpensesApi(api_client)
    expense_id = 'expense_id_example' # str | 

    try:
        # Get
        api_response = api_instance.get_expenses_expense_id_get(expense_id)
        print("The response of ExpensesApi->get_expenses_expense_id_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExpensesApi->get_expenses_expense_id_get: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **expense_id** | **str**|  | 

### Return type

[**Expense**](Expense.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_expenses_get**
> List[Expense] get_expenses_get()

Get

### Example

```python
import time
import os
import tdc_api_client
from tdc_api_client.models.expense import Expense
from tdc_api_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = tdc_api_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with tdc_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = tdc_api_client.ExpensesApi(api_client)

    try:
        # Get
        api_response = api_instance.get_expenses_get()
        print("The response of ExpensesApi->get_expenses_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExpensesApi->get_expenses_get: %s\n" % e)
```



### Parameters
This endpoint does not need any parameter.

### Return type

[**List[Expense]**](Expense.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_project_expenses_project_id_expenses_get**
> List[Expense] get_project_expenses_project_id_expenses_get(project_id)

Get Project

### Example

```python
import time
import os
import tdc_api_client
from tdc_api_client.models.expense import Expense
from tdc_api_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = tdc_api_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with tdc_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = tdc_api_client.ExpensesApi(api_client)
    project_id = 'project_id_example' # str | 

    try:
        # Get Project
        api_response = api_instance.get_project_expenses_project_id_expenses_get(project_id)
        print("The response of ExpensesApi->get_project_expenses_project_id_expenses_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExpensesApi->get_project_expenses_project_id_expenses_get: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **str**|  | 

### Return type

[**List[Expense]**](Expense.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_expenses_post**
> post_expenses_post(expense)

Post

### Example

```python
import time
import os
import tdc_api_client
from tdc_api_client.models.expense import Expense
from tdc_api_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = tdc_api_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with tdc_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = tdc_api_client.ExpensesApi(api_client)
    expense = tdc_api_client.Expense() # Expense | 

    try:
        # Post
        api_instance.post_expenses_post(expense)
    except Exception as e:
        print("Exception when calling ExpensesApi->post_expenses_post: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **expense** | [**Expense**](Expense.md)|  | 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

