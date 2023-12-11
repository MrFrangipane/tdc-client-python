# tdc_api_client.ExpensesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**expenses_delete**](ExpensesApi.md#expenses_delete) | **DELETE** /expenses/ | 
[**expenses_project_id_expenses_get**](ExpensesApi.md#expenses_project_id_expenses_get) | **GET** /expenses/{project_id}/expenses | 
[**expenses_project_id_expenses_post**](ExpensesApi.md#expenses_project_id_expenses_post) | **POST** /expenses/{project_id}/expenses | 
[**expenses_put**](ExpensesApi.md#expenses_put) | **PUT** /expenses/ | 


# **expenses_delete**
> expenses_delete(expense)



### Example

* Bearer Authentication (HTTPBearer):
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

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = tdc_api_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with tdc_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = tdc_api_client.ExpensesApi(api_client)
    expense = tdc_api_client.Expense() # Expense | 

    try:
        # 
        api_instance.expenses_delete(expense)
    except Exception as e:
        print("Exception when calling ExpensesApi->expenses_delete: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **expense** | [**Expense**](Expense.md)|  | 

### Return type

void (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **expenses_project_id_expenses_get**
> List[Expense] expenses_project_id_expenses_get(project_id)



### Example

* Bearer Authentication (HTTPBearer):
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

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = tdc_api_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with tdc_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = tdc_api_client.ExpensesApi(api_client)
    project_id = 'project_id_example' # str | 

    try:
        # 
        api_response = api_instance.expenses_project_id_expenses_get(project_id)
        print("The response of ExpensesApi->expenses_project_id_expenses_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExpensesApi->expenses_project_id_expenses_get: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **str**|  | 

### Return type

[**List[Expense]**](Expense.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **expenses_project_id_expenses_post**
> Expense expenses_project_id_expenses_post(project_id, expense)



### Example

* Bearer Authentication (HTTPBearer):
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

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = tdc_api_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with tdc_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = tdc_api_client.ExpensesApi(api_client)
    project_id = 'project_id_example' # str | 
    expense = tdc_api_client.Expense() # Expense | 

    try:
        # 
        api_response = api_instance.expenses_project_id_expenses_post(project_id, expense)
        print("The response of ExpensesApi->expenses_project_id_expenses_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExpensesApi->expenses_project_id_expenses_post: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **str**|  | 
 **expense** | [**Expense**](Expense.md)|  | 

### Return type

[**Expense**](Expense.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **expenses_put**
> expenses_put(expense)



### Example

* Bearer Authentication (HTTPBearer):
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

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure Bearer authorization: HTTPBearer
configuration = tdc_api_client.Configuration(
    access_token = os.environ["BEARER_TOKEN"]
)

# Enter a context with an instance of the API client
with tdc_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = tdc_api_client.ExpensesApi(api_client)
    expense = tdc_api_client.Expense() # Expense | 

    try:
        # 
        api_instance.expenses_put(expense)
    except Exception as e:
        print("Exception when calling ExpensesApi->expenses_put: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **expense** | [**Expense**](Expense.md)|  | 

### Return type

void (empty response body)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

