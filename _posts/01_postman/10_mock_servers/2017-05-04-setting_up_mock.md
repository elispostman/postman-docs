---
categories:
  - "postman"
  - "mock_servers"
title: "Setting up a mock server"
page_id: "setting_up_mock"
warning: false
---

### Simulate a back end with Postman's mock servers

Throughout the development process, delays on the front end or back end can hold up dependent teams from completing their work efficiently.  

Using Postman's mock servers, front-end developers can simulate each endpoint in a Postman Collection (and corresponding environment) to view the potential responses, without actually spinning up a back end.

Front-end, back-end and API teams can now work in parallel, freeing up developers who were previously delayed as a result of these dependencies.

### Setting up the mock

Developers can mock a request and response in Postman before sending the actual request or setting up a single endpoint to return the response. Establishing an [example](/docs/postman/collections/examples) during the earliest phase of API development requires clear communication between team members, aligns their expectations, and means developers and testers can get started more quickly.

There are two ways to create a mock: 

  1. [using the Postman app](/docs/postman/mock_servers/mocking_with_examples)
  2. [using the Postman Pro API](/docs/postman/mock_servers/mock_with_api)
  
Once the mock has been created, Postman Pro and Enterprise users can share the mock with their team for review and collaboration. This is accomplished by [sharing the underlying collection](/docs/postman/team_library/sharing#sharing-collections) with the team or specific team members, providing permissions to edit or view.

### HTTP access control (CORS)

Not only can you make requests to mock endpoints using the Postman app, you can also rely on a mock using a browser. A web browser makes a cross-origin HTTP request when requesting a resource from a domain, protocol, or port that's different from its own. For security reasons, [cross-origin resource sharing (CORS)](https://developer.mozilla.org/en-US/docs/Web/HTTP/Access_control_CORS){:target="_blank"} is a standard that defines a way in which a browser and server can interact securely. In this case, we are referring to how a web browser interacts with the mock endpoints hosted on the Postman server.

CORS is enabled for Postman mock servers which means you can stub your web apps with mocked data using the mock endpoints. In other words, development or production web apps can make requests to the Postman mock endpoint you just created and receive an example response.

### Free mock server calls with your Postman account

Your Postman account gives you a limited number of free mock server calls per month. You can check your usage limits through the [Postman Pro API](https://docs.api.getpostman.com) or the [account usage page](https://go.pstmn.io/postman-account-limits).
