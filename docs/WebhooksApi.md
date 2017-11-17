# vericite_lms_client.WebhooksApi

All URIs are relative to *https://localhost/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**create_webhook**](WebhooksApi.md#create_webhook) | **POST** /webhooks | 
[**delete_webhook**](WebhooksApi.md#delete_webhook) | **DELETE** /webhooks | 
[**get_webhooks**](WebhooksApi.md#get_webhooks) | **GET** /webhooks | 


# **create_webhook**
> Webhook create_webhook(consumer, consumer_secret, webhook)



Create/update webhook for event

### Example 
```python
from __future__ import print_function
import time
import vericite_lms_client
from vericite_lms_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = vericite_lms_client.WebhooksApi()
consumer = 'consumer_example' # str | the consumer
consumer_secret = 'consumer_secret_example' # str | the consumer secret
webhook = vericite_lms_client.Webhook() # Webhook | 

try: 
    api_response = api_instance.create_webhook(consumer, consumer_secret, webhook)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling WebhooksApi->create_webhook: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **consumer** | **str**| the consumer | 
 **consumer_secret** | **str**| the consumer secret | 
 **webhook** | [**Webhook**](Webhook.md)|  | 

### Return type

[**Webhook**](Webhook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **delete_webhook**
> Webhook delete_webhook(consumer, consumer_secret, webhook)



Delete webhook for event

### Example 
```python
from __future__ import print_function
import time
import vericite_lms_client
from vericite_lms_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = vericite_lms_client.WebhooksApi()
consumer = 'consumer_example' # str | the consumer
consumer_secret = 'consumer_secret_example' # str | the consumer secret
webhook = vericite_lms_client.Webhook() # Webhook | 

try: 
    api_response = api_instance.delete_webhook(consumer, consumer_secret, webhook)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling WebhooksApi->delete_webhook: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **consumer** | **str**| the consumer | 
 **consumer_secret** | **str**| the consumer secret | 
 **webhook** | [**Webhook**](Webhook.md)|  | 

### Return type

[**Webhook**](Webhook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_webhooks**
> list[Webhook] get_webhooks(consumer, consumer_secret, event=event)



Retrieves webhooks for the consumer

### Example 
```python
from __future__ import print_function
import time
import vericite_lms_client
from vericite_lms_client.rest import ApiException
from pprint import pprint

# create an instance of the API class
api_instance = vericite_lms_client.WebhooksApi()
consumer = 'consumer_example' # str | the consumer
consumer_secret = 'consumer_secret_example' # str | the consumer secret
event = 'event_example' # str | optional event filter (optional)

try: 
    api_response = api_instance.get_webhooks(consumer, consumer_secret, event=event)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling WebhooksApi->get_webhooks: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **consumer** | **str**| the consumer | 
 **consumer_secret** | **str**| the consumer secret | 
 **event** | **str**| optional event filter | [optional] 

### Return type

[**list[Webhook]**](Webhook.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

