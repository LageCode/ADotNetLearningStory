# A .NET Learning Story  

## Web Services  

### Web API with ASP.NET Core  

API clients communicate with the server over HTTP, and the two exchange information by using a data format such as JSON or XML.  

REpresentational State Transfer (REST) is an architectural style for building web services.

REST requests are made over HTTP. They use the same HTTP verbs that web browsers use to retrieve webpages and send data to servers: 

- `GET`: Retrieve data from WS.
- `POST`: Create a new item of data on the WS.
- `PUT`: Update an item of data on the WS.
- `DELETE`: Delete an item of data on the WS.

Web services that adhere to REST are called RESTful and are defined through:

- a base URL.
- HTTP methods, such as `GET`, `POST`, `PUT`, `DELETE`.
- a media type for the data, such as JSON or XML.

Sometimes, an API needs to provide services for different but related things; we use routing to map URIs (Uniform Resource Identifiers) to logical divisions in our code, so that requests are routed to corresponding controller.

> [Sources](https://learn.microsoft.com/en-us/training/modules/build-web-api-aspnet-core/2-what-is-rest-in-aspnet)  