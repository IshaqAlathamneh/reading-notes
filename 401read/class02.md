# Class 02

## Questions
1. What’s the difference between PUT and PATCH?

    PUT is a method of modifying resource where the client sends data that updates the entire resource. It is used to set an entity’s information completely.PUT overwrites the entire entity if it already exists, and creates a new resource if it doesn’t exist.Unlike PUT, PATCH applies a partial update to the resource.This means that you are only required to send the data that you want to update, and it won’t affect or change anything else. 
1. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server
    * [Nock](https://github.com/nock/nock)
    * [MockServer](https://www.mock-server.com/)
    * [Postman](https://learning.postman.com/docs/designing-and-developing-your-api/mocking-data/setting-up-mock/)
1. Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

    apidoc and swagger are two nice projects which are focusing on documentation of APIs. This project is a middle tier which tries to bring them   together in a sense that:
    It uses apidoc to convert inline documentation comments into json schema and later convert it to swagger json schema.
1. Compare and contrast SOAP and ReST

    SOAP is a protocol, and REST is an architectural style. A REST API can actually utilize the SOAP protocol, just like it can use HTTP.

## Notes
1. Which 3 things had you heard about previously and now have better clarity on?
    * node.js
    * npm
    * express
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    * http status codes
    * supertest
    * should & cookie-parser
1. What are you most excited about trying to implement or see how it works?

    thinking how they will make you experience much easier.