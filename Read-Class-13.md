# CRUD

## 1. In your own words, describe what each group of status code represents:

* 100’s = *These are informative status codes that typically indicate the client that the header portion of the request has been received and that the server will attempt to fulfill the client's transmission request. For example, you might use an alternative protocol or inform the client that their request will fail before delivering the body.*
* 200’s = *These are the keys to success. They inform the customer that their request has been granted. Asynchronous request processing (202), on the other hand, does not imply that the request was successfully processed; rather, it means that it fulfilled all validation criteria at the time of sending.*
* 300’s = *This is a list of redirection codes. They inform the client that the requested resource is no longer accessible at the expected location. This might be for a variety of reasons, including temporary or permanent relocation, but the customer must submit a request to the new location.*
* 400’s = *These are the error codes for clients. They're all about incorrect requests made to a server by a client. There are numerous reasons for this, including timeouts, incorrect URIs, and insufficient authentication. If a client sends erroneous data, the request should be retried after double-checking the input parameters.*
* 500’s = *The server error codes are shown below. They frequently signal issues with overburdened servers or inaccessible servers behind proxies, but they can also be directly connected to client requests that cause server error exceptions. Temporary or permanent mistakes might occur. Retrying the same request is usually the best option for the customer.*

## 2. What is a status code 202?

*202 Accepted,Asynchronous processing is frequently utilized. This code informs the client that the request was legitimate, but that it will be processed at a later time. The response body should contain either a URL to the completed resource with information about when it will be accessible, or a URL to a monitoring endpoint that notifies the client when the resource is ready.*

## 3. What is a status code 308?

*308 Permanent Redirect,This instructs the client to access the resource through a different URL rather than the current one. When we have several endpoints for a single resource but don't want to implement reading from all of them, this is useful.*

## 4. What code would you use if an update didn’t return data to a client?

*204 No Content.*

## 5. What code would you use if a resource used to exist but no longer does?

*410 Gone.*

## 6. What is the ‘Forbidden’ status code?

*403 Forbidden,The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.*

## Things I want to know more about

* more about API, mongo db and react
