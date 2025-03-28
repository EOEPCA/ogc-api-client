# ogcapi_processes_client.JobListApi

All URIs are relative to *http://example.org/ogc*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_jobs**](JobListApi.md#get_jobs) | **GET** /jobs | retrieve the list of jobs.


# **get_jobs**
> JobList get_jobs()

retrieve the list of jobs.

Lists available jobs.

For more information, see [Section 11](https://docs.ogc.org/is/18-062r2/18-062r2.html#sc_job_list).


### Example


```python
import ogcapi_processes_client
from ogcapi_processes_client.models.job_list import JobList
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
    api_instance = ogcapi_processes_client.JobListApi(api_client)

    try:
        # retrieve the list of jobs.
        api_response = api_instance.get_jobs()
        print("The response of JobListApi->get_jobs:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling JobListApi->get_jobs: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**JobList**](JobList.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | A list of jobs for this process. |  -  |
**404** | The requested URI was not found. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

