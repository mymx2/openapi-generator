# petstore_api.AnotherFakeApi

All URIs are relative to *http://petstore.swagger.io:80/v2*

Method | HTTP request | Description
------------- | ------------- | -------------
[**call_123_test_special_tags**](AnotherFakeApi.md#call_123_test_special_tags) | **PATCH** /another-fake/dummy | To test special tags


# **call_123_test_special_tags**
> Client call_123_test_special_tags(client)

To test special tags

To test special tags and operation ID starting with number

### Example


```python
import time
import os
import petstore_api
from petstore_api.models.client import Client
from petstore_api.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://petstore.swagger.io:80/v2
# See configuration.py for a list of all supported configuration parameters.
configuration = petstore_api.Configuration(
    host = "http://petstore.swagger.io:80/v2"
)


# Enter a context with an instance of the API client
async with petstore_api.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = petstore_api.AnotherFakeApi(api_client)
    client = petstore_api.Client() # Client | client model

    try:
        # To test special tags
        api_response = await api_instance.call_123_test_special_tags(client)
        print("The response of AnotherFakeApi->call_123_test_special_tags:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling AnotherFakeApi->call_123_test_special_tags: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **client** | [**Client**](Client.md)| client model | 

### Return type

[**Client**](Client.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | successful operation |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

