**AWS API Gateway to lambda (build a REST API)**

This code is an AWS Lambda function that can be triggered by an HTTP request through an API Gateway.

The function receives a request that includes query string parameters, which are then parsed out in lines 7-9 to extract the values of the transaction ID, type, and amount.

Then, the function constructs a response object that includes these values along with a message that says 'Hello from Lambda land'. This response object is constructed as a dictionary in line 13-16.

Next, the function constructs an HTTP response object that includes the constructed transaction response object and appropriate headers to indicate that the response body is in JSON format. This response object is constructed as a dictionary in lines 18-21.

Finally, the function returns the constructed HTTP response object, which is sent back to the client that made the original HTTP request.

Rest API - REST (Representational State Transfer) API is an architectural style for building web services. It is based on the HTTP protocol and uses HTTP methods like GET, POST, PUT, DELETE, etc. to communicate between client and server.

A RESTful API is designed to be stateless, meaning that the server does not store any session data about the client. Instead, each request from the client contains all the necessary information to complete the request. The response from the server contains all the necessary information to complete the request. The response from the server contains the requested data in a format that is easy for the client to parse, such as JSON or XML.

AWS API Gateway - AWS API Gateway is a fully managed service that allows developers to create, publish, maintain, monitor, and secure REST and WebSocket APIs at any scale. It acts as a front-end service for your APIs and can interact with various backend services like AWS Lambda, EC2, S3, and more. API Gateway makes it easy to expose your APIs to external developers, partners, or internal teams.
