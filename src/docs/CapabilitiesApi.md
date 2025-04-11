# ogc_api_client.CapabilitiesApi

All URIs are relative to *http://example.org/ogc*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_landing_page**](CapabilitiesApi.md#get_landing_page) | **GET** / | landing page of this API


# **get_landing_page**
> LandingPage get_landing_page()

landing page of this API

The landing page provides links to the:
  * The APIDefinition (no fixed path),
  * The Conformance statements (path /conformance),
  * The processes metadata (path /processes),
  * The endpoint for job monitoring (path /jobs).

For more information, see [Section 7.2](https://docs.ogc.org/is/18-062r2/18-062r2.html#sc_landing_page).

### Example


```python
import ogc_api_client
from ogc_api_client.models.landing_page import LandingPage
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
    api_instance = ogc_api_client.CapabilitiesApi(api_client)

    try:
        # landing page of this API
        api_response = api_instance.get_landing_page()
        print("The response of CapabilitiesApi->get_landing_page:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling CapabilitiesApi->get_landing_page: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**LandingPage**](LandingPage.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json, text/html

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | The landing page provides links to the API definition (link relations &#x60;service-desc&#x60; and &#x60;service-doc&#x60;), the Conformance declaration (path &#x60;/conformance&#x60;, link relation &#x60;http://www.opengis.net/def/rel/ogc/1.0/conformance&#x60;), and to other resources. |  -  |
**500** | A server error occurred. |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

