# ogcapi_processes_client.ProcessDescriptionApi

All URIs are relative to *http://example.org/ogc*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_process_description**](ProcessDescriptionApi.md#get_process_description) | **GET** /processes/{processID} | retrieve a process description


# **get_process_description**
> Process get_process_description(process_id)

retrieve a process description

The process description contains information about inputs and outputs and a link to the execution-endpoint for the process. The Core does not mandate the use of a specific process description to specify the interface of a process. That said, the Core requirements class makes the following recommendation:

Implementations SHOULD consider supporting the OGC process description.

For more information, see [Section 7.10](https://docs.ogc.org/is/18-062r2/18-062r2.html#sc_process_description).


### Example


```python
import ogcapi_processes_client
from ogcapi_processes_client.models.process import Process
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
    api_instance = ogcapi_processes_client.ProcessDescriptionApi(api_client)
    process_id = 'process_id_example' # str | 

    try:
        # retrieve a process description
        api_response = api_instance.get_process_description(process_id)
        print("The response of ProcessDescriptionApi->get_process_description:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ProcessDescriptionApi->get_process_description: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **process_id** | **str**|  | 

### Return type

[**Process**](Process.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | A process description. |  -  |
**404** | The requested URI was not found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

