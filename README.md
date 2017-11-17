# vericite_lms_client
No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)

This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: 1.0.0
- Package version: 1.0.0
- Build package: io.swagger.codegen.languages.PythonClientCodegen

## Requirements.

Python 2.7 and 3.4+

## Installation & Usage
### pip install

If the python package is hosted on Github, you can install directly from Github

```sh
pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
```
(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)

Then import the package:
```python
import vericite_lms_client 
```

### Setuptools

Install via [Setuptools](http://pypi.python.org/pypi/setuptools).

```sh
python setup.py install --user
```
(or `sudo python setup.py install` to install the package for all users)

Then import the package:
```python
import vericite_lms_client
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```python
from __future__ import print_function
import time
import vericite_lms_client
from vericite_lms_client.rest import ApiException
from pprint import pprint
# create an instance of the API class
api_instance = vericite_lms_client.AssignmentsApi()
context_id = 'context_id_example' # str | Context ID
assignment_id = 'assignment_id_example' # str | ID of assignment
consumer = 'consumer_example' # str | the consumer
consumer_secret = 'consumer_secret_example' # str | the consumer secret
assignment_data = vericite_lms_client.AssignmentData() # AssignmentData | 
encrypted = true # bool | Flag to indicate encryption (optional)

try:
    api_response = api_instance.create_update_assignment(context_id, assignment_id, consumer, consumer_secret, assignment_data, encrypted=encrypted)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling AssignmentsApi->create_update_assignment: %s\n" % e)

```

## Documentation for API Endpoints

All URIs are relative to *https://localhost/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AssignmentsApi* | [**create_update_assignment**](docs/AssignmentsApi.md#create_update_assignment) | **POST** /assignments/{contextID}/{assignmentID} | 
*ReportsApi* | [**get_report_urls**](docs/ReportsApi.md#get_report_urls) | **GET** /reports/urls/{contextID} | 
*ReportsApi* | [**get_scores**](docs/ReportsApi.md#get_scores) | **GET** /reports/scores/{contextID} | 
*ReportsApi* | [**submit_request**](docs/ReportsApi.md#submit_request) | **POST** /reports/submit/request/{contextID}/{assignmentID}/{userID} | 
*WebhooksApi* | [**create_webhook**](docs/WebhooksApi.md#create_webhook) | **POST** /webhooks | 
*WebhooksApi* | [**delete_webhook**](docs/WebhooksApi.md#delete_webhook) | **DELETE** /webhooks | 
*WebhooksApi* | [**get_webhooks**](docs/WebhooksApi.md#get_webhooks) | **GET** /webhooks | 


## Documentation For Models

 - [AssignmentData](docs/AssignmentData.md)
 - [Error](docs/Error.md)
 - [ExternalContentData](docs/ExternalContentData.md)
 - [ExternalContentUploadInfo](docs/ExternalContentUploadInfo.md)
 - [ReportMetaData](docs/ReportMetaData.md)
 - [ReportScoreReponse](docs/ReportScoreReponse.md)
 - [ReportURLLinkResponse](docs/ReportURLLinkResponse.md)
 - [Webhook](docs/Webhook.md)


## Documentation For Authorization

 All endpoints do not require authorization.


## Author


