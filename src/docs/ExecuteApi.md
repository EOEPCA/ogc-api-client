# ogc_api_client.ExecuteApi

All URIs are relative to *http://example.org/ogc*

Method | HTTP request | Description
------------- | ------------- | -------------
[**execute**](ExecuteApi.md#execute) | **POST** /processes/{processID}/execution | execute a process.


# **execute**
> Execute200Response execute(process_id, execute)

execute a process.

Create a new job.

For more information, see [Section 7.11](https://docs.ogc.org/is/18-062r2/18-062r2.html#sc_create_job).


### Example


```python
import ogc_api_client
from ogc_api_client.models.execute import Execute
from ogc_api_client.models.execute200_response import Execute200Response
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
    api_instance = ogc_api_client.ExecuteApi(api_client)
    process_id = 'process_id_example' # str | 
    execute = ogc_api_client.Execute() # Execute | Mandatory execute request JSON

    try:
        # execute a process.
        api_response = api_instance.execute(process_id, execute)
        print("The response of ExecuteApi->execute:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling ExecuteApi->execute: %s\n" % e)
```



### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **process_id** | **str**|  | 
 **execute** | [**Execute**](Execute.md)| Mandatory execute request JSON | 

### Return type

[**Execute200Response**](Execute200Response.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: /*, application/json, text/html

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Result of synchronous execution |  -  |
**201** | Started asynchronous execution. Created job. |  * Location - URL to check the status of the execution/job. <br>  * Preference-Applied - The preference applied to execute the process asynchronously (see. RFC 2740). <br>  |
**404** | The requested URI was not found. |  -  |
**500** | A server error occurred. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

