# ogc_api_client.DismissApi

All URIs are relative to *http://example.org/ogc*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dismiss**](DismissApi.md#dismiss) | **DELETE** /jobs/{jobId} | cancel a job execution, remove a finished job


# **dismiss**
> StatusInfo dismiss(job_id)

cancel a job execution, remove a finished job

Cancel a job execution and remove it from the jobs list.

For more information, see [Section 13](https://docs.ogc.org/is/18-062r2/18-062r2.html#Dismiss).


### Example


```python
import ogc_api_client
from ogc_api_client.models.status_info import StatusInfo
from ogc_api_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://example.org/ogc
# See configuration.py for a list of all supported configuration parameters.
configuration = ogc_api_client.Configuration(
    host = "http://example.org/ogc"
)


# Enter a context with an instance of the API client
with ogc_api_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = ogc_api_client.DismissApi(api_client)
    job_id = 'job_id_example' # str | local identifier of a job

    try:
        # cancel a job execution, remove a finished job
        api_response = api_instance.dismiss(job_id)
        print("The response of DismissApi->dismiss:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling DismissApi->dismiss: %s\n" % e)
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

