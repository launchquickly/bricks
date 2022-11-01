# JSON over HTTP Server (gorilla/mux)

Web server that supports API requests as JSON over the HTTP protocol using [gorilla/mux](https://github.com/gorilla/mux) library to provide support for RESTful routes

examples consist of 3 basic steps for each endpoint:

1. JSON request to enpoint that is unmarshalled into a struct
1. handler logic associated with logic is invoked
1. result is marshalled into JSON and returned as the response

supporting tests assert the following types of conditions:

1. correct endpoint is mapped to appropriate endpoint route
1. correct handler logic is mapped to specific endpoint route
1. expected HTTP response code is returned based on request supplied
1. expected response body is returned based on request supplied
1. expected error conditions are handled