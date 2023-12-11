# tdc_api_client.ProjectsApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**projects_delete**](ProjectsApi.md#projects_delete) | **DELETE** /projects/ | 
[**projects_get**](ProjectsApi.md#projects_get) | **GET** /projects/ | 
[**projects_post**](ProjectsApi.md#projects_post) | **POST** /projects/ | 
[**projects_put**](ProjectsApi.md#projects_put) | **PUT** /projects/ | 


# **projects_delete**
> projects_delete(project)



### Example

* Bearer Authentication (HTTPBearer):
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
    api_instance = tdc_api_client.ProjectsApi(api_client)
    project = tdc_api_client.Project() # Project | 

    try:
        # 
        api_instance.projects_delete(project)
    except Exception as e:
        print("Exception when calling ProjectsApi->projects_delete: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | [**Project**](Project.md)|  | 

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

# **projects_get**
> List[Project] projects_get()



### Example

* Bearer Authentication (HTTPBearer):
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
    api_instance = tdc_api_client.ProjectsApi(api_client)

    try:
        # 
        api_response = api_instance.projects_get()
        print("The response of ProjectsApi->projects_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->projects_get: %s\n" % e)
```



### Parameters
This endpoint does not need any parameter.

### Return type

[**List[Project]**](Project.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **projects_post**
> Project projects_post()



### Example

* Bearer Authentication (HTTPBearer):
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
    api_instance = tdc_api_client.ProjectsApi(api_client)

    try:
        # 
        api_response = api_instance.projects_post()
        print("The response of ProjectsApi->projects_post:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProjectsApi->projects_post: %s\n" % e)
```



### Parameters
This endpoint does not need any parameter.

### Return type

[**Project**](Project.md)

### Authorization

[HTTPBearer](../README.md#HTTPBearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **projects_put**
> projects_put(project)



### Example

* Bearer Authentication (HTTPBearer):
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
    api_instance = tdc_api_client.ProjectsApi(api_client)
    project = tdc_api_client.Project() # Project | 

    try:
        # 
        api_instance.projects_put(project)
    except Exception as e:
        print("Exception when calling ProjectsApi->projects_put: %s\n" % e)
```



### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project** | [**Project**](Project.md)|  | 

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

