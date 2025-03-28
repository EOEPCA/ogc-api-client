# ogcapi_processes_client.ResultApi

All URIs are relative to *http://example.org/ogc*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_result**](ResultApi.md#get_result) | **GET** /jobs/{jobId}/results | retrieve the result(s) of a job


# **get_result**
> Dict[str, InlineOrRefData] get_result(job_id)

retrieve the result(s) of a job

Lists available results of a job. In case of a failure, lists exceptions instead.

For more information, see [Section 7.13](https://docs.ogc.org/is/18-062r2/18-062r2.html#sc_retrieve_job_results).


### Example


```python
import ogcapi_processes_client
from ogcapi_processes_client.models.inline_or_ref_data import InlineOrRefData
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
    api_instance = ogcapi_processes_client.ResultApi(api_client)
    job_id = 'job_id_example' # str | local identifier of a job

    try:
        # retrieve the result(s) of a job
        api_response = api_instance.get_result(job_id)
        print("The response of ResultApi->get_result:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ResultApi->get_result: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **job_id** | **str**| local identifier of a job | 

### Return type

[**Dict[str, InlineOrRefData]**](InlineOrRefData.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | The results of a job. |  -  |
**404** | The requested URI was not found. |  -  |
**500** | A server error occurred. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

