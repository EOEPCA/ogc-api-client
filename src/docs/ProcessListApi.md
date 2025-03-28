# ogcapi_processes_client.ProcessListApi

All URIs are relative to *http://example.org/ogc*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_processes**](ProcessListApi.md#get_processes) | **GET** /processes | retrieve the list of available processes


# **get_processes**
> ProcessList get_processes()

retrieve the list of available processes

The list of processes contains a summary of each process the OGC API - Processes offers, including the link to a more detailed description of the process.

For more information, see [Section 7.9](https://docs.ogc.org/is/18-062r2/18-062r2.html#sc_process_list).


### Example


```python
import ogcapi_processes_client
from ogcapi_processes_client.models.process_list import ProcessList
from ogcapi_processes_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://example.org/ogc
# See configuration.py for a list of all supported configuration parameters.
configuration = ogcapi_processes_client.Configuration(
    host = "http://example.org/ogc"
)


# Enter a context with an instance of the API client
with ogcapi_processes_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ogcapi_processes_client.ProcessListApi(api_client)

    try:
        # retrieve the list of available processes
        api_response = api_instance.get_processes()
        print("The response of ProcessListApi->get_processes:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProcessListApi->get_processes: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**ProcessList**](ProcessList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Information about the available processes |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

