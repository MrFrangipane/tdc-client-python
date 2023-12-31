# tdc_api_client.UsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**users_me_get**](UsersApi.md#users_me_get) | **GET** /users/me | 


# **users_me_get**
> User users_me_get()



### Example

* Bearer Authentication (HTTPBearer):
```python
import time
import os
import tdc_api_client
from tdc_api_client.models.user import User
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
    api_instance = tdc_api_client.UsersApi(api_client)

    try:
        # 
        api_response = api_instance.users_me_get()
        print("The response of UsersApi->users_me_get:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling UsersApi->users_me_get: %s\n" % e)
```



### Parameters
This endpoint does not need any parameter.

### Return type

[**User**](User.md)

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

