# ogcapi_processes_client.StatusApi

All URIs are relative to *http://example.org/ogc*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_status**](StatusApi.md#get_status) | **GET** /jobs/{jobId} | retrieve the status of a job


# **get_status**
> StatusInfo get_status(job_id)

retrieve the status of a job

Shows the status of a job.

 For more information, see [Section 7.12](https://docs.ogc.org/is/18-062r2/18-062r2.html#sc_retrieve_status_info).


### Example


```python
import ogcapi_processes_client
from ogcapi_processes_client.models.status_info import StatusInfo
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
    api_instance = ogcapi_processes_client.StatusApi(api_client)
    job_id = 'job_id_example' # str | local identifier of a job

    try:
        # retrieve the status of a job
        api_response = api_instance.get_status(job_id)
        print("The response of StatusApi->get_status:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling StatusApi->get_status: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **job_id** | **str**| local identifier of a job | 

### Return type

[**StatusInfo**](StatusInfo.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | The status of a job. |  -  |
**404** | The requested URI was not found. |  -  |
**500** | A server error occurred. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

