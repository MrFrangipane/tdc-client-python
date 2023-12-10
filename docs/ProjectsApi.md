# tdc_api_client.ProjectsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_projects_get**](ProjectsApi.md#get_projects_get) | **GET** /projects/ | Get
[**new_projects_post**](ProjectsApi.md#new_projects_post) | **POST** /projects/ | New
[**remove_projects_delete**](ProjectsApi.md#remove_projects_delete) | **DELETE** /projects/ | Remove
[**update_projects_put**](ProjectsApi.md#update_projects_put) | **PUT** /projects/ | Update


# **get_projects_get**
> List[Project] get_projects_get()

Get

### Example

```python
import time
import os
import tdc_api_client
from tdc_api_client.models.project import Project
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
    api_instance = tdc_api_client.ProjectsApi(api_client)

    try:
        # Get
        api_response = api_instance.get_projects_get()
        print("The response of ProjectsApi->get_projects_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->get_projects_get: %s\n" % e)
```



### Parameters
This endpoint does not need any parameter.

### Return type

[**List[Project]**](Project.md)

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

# **new_projects_post**
> Project new_projects_post()

New

### Example

```python
import time
import os
import tdc_api_client
from tdc_api_client.models.project import Project
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
    api_instance = tdc_api_client.ProjectsApi(api_client)

    try:
        # New
        api_response = api_instance.new_projects_post()
        print("The response of ProjectsApi->new_projects_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->new_projects_post: %s\n" % e)
```



### Parameters
This endpoint does not need any parameter.

### Return type

[**Project**](Project.md)

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

# **remove_projects_delete**
> remove_projects_delete(project)

Remove

### Example

```python
import time
import os
import tdc_api_client
from tdc_api_client.models.project import Project
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
    api_instance = tdc_api_client.ProjectsApi(api_client)
    project = tdc_api_client.Project() # Project | 

    try:
        # Remove
        api_instance.remove_projects_delete(project)
    except Exception as e:
        print("Exception when calling ProjectsApi->remove_projects_delete: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | [**Project**](Project.md)|  | 

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

# **update_projects_put**
> update_projects_put(project)

Update

### Example

```python
import time
import os
import tdc_api_client
from tdc_api_client.models.project import Project
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
    api_instance = tdc_api_client.ProjectsApi(api_client)
    project = tdc_api_client.Project() # Project | 

    try:
        # Update
        api_instance.update_projects_put(project)
    except Exception as e:
        print("Exception when calling ProjectsApi->update_projects_put: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | [**Project**](Project.md)|  | 

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

