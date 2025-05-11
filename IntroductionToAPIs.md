# [Introduction to APIs](#introduction-to-apis)

## [What is an Application Programming Interface?](#what-is-an-application-programming-interface)
An application programming interface (API) is an intermediary through which two software components communicate to share data and to get useful work done. As the name implies, exchanging information is possible because of the presence of a software interface between these components. The software components can reside on the same or different machines connected through a network.

Using an API, an application can request services from another application without understanding the architecture of other applications. The only thing the requesting application should know is how to place the request, in other words, it should understand the interface for placing the request.

---

## [Benefits of APIs](#benefits-of-apis)
Some major advantages of using APIs are as follows:

* **Complexity abstraction:** New services are often complex, with many moving parts. APIs help us to hide all that complexity within a service away from the consumer. Doing so has many benefits, such as the flexibility to change the internals of the service without changing the interface. With APIs, the caller of the service can focus on their application without worrying about the internal complexity of the calling service. The caller only has to focus on the interface and return data from the callee.

* **Improved modularity:** APIs aid the microservices architecture of applications by further breaking down applications into subsets of services. Developers use this modularity to design a flexible, maintainable, and reusable application.

* **Efficient development:** APIs have reduced the development time and the number of bugs by preventing developers from having to rewrite code for the same functionality. With APIs, developers can request services by making a simple call, without the need to rewrite code from scratch.

* **API expedites digitization:** APIs were critical for expedited digitization, especially since the start COVID-19. According to the Moesif summary of a McKinsey report: "Coronavirus has acted as an accelerant on companies offering digital products and services. Across all business areas, digital adoption has accelerated to such a degree that it’s the equivalent of fast-forwarding six years where 60% of all businesses in the US employ digital processes".

* **Controlled accessibility:** APIs provide applications with the flexibility to share limited data or information with a restricted number of users. Other techniques can be used to throttle the frequency of service usage.

---

## [Types of APIs](#types-of-apis)
The APIs can be divided into four types based on users and their access levels, as shown below:

- **Public APIs** are intended for developers to access publicly available data or services. Public APIs are freely accessible, but are limited to a few calls for a certain time period.

- **Private APIs** are designed for internal use only. The developers working within the company can use them to improve their products and services. They have the highest level of access and can see and update the complexity of the back-end system.

- **Partner APIs** are for users that have business relationships with the company that owns the APIs. These APIs have more robust security measures than public APIs. Generally, they are purpose-specific—such as giving access to a prepaid service—and are a widely used pattern in the ecosystem.

- **Composite APIs** allow developers to bundle the request call for different services and get a unified response from different requested resources. Composite APIs are handy when a developer needs data from different servers without making a separate API call to each server. It makes the system work faster and more efficiently by reducing the number of API calls and complexity.

---

## [API Types Overview](#api-types-overview)


| API Type      | Authentication Type                          | Potential Users                     | Examples                          |
|---------------|---------------------------------------------|-------------------------------------|-----------------------------------|
| Public APIs   | Publicly accessible with API keys           | B2C (business-to-consumer)         | Google Maps, Weather APIs         |
| Private APIs  | No authentication                            | B2B (business-to-business), B2C, B2E (business-to-employee) | Amazon S3 API for data storage |
| Partner APIs  | Authorized access with access tokens/license | B2B, B2C                           | Amazon APIs for partners          |
| Composite APIs| Depends on the connected API’s authentication| B2B, B2C, B2E                      | Payment APIs (Stripe, PayPal)    |

---


## [API gateway](#api-gateway)
Modern software applications prefer microservices over monolithic architecture. This is because their rich features require multiple services to process tasks with added flexibility. The microservice architecture is easy to manage and develop and provides modularity to the application compared to the monolithic.

In a scenario where a client application must interact with multiple microservices at a time, a typical approach would be to make a separate API call for each microservice. This impacts resource consumption, performance, and task time. The API gateway comes in to help by acting as a single entry point for all the API requests. It sits between the microservices and clients, acting as a gateway.

![image](https://github.com/user-attachments/assets/116ddd4a-128c-4dd5-a4ba-9d1877949a5e)

The API gateway takes the client’s calls and routes them to the appropriate microservice by processing the parameters in composite API calls. It retrieves the responses from all microservices and sends a unified response to the client’s requests. Most applications depend on APIs; therefore, cyber attacks target them because they can expose valuable users and system data. It is of utmost importance to protect APIs from unauthorized access. An API gateway plays the following essential roles:
- It provides security, authentication, and rate limiting to protect APIs from overuse.
- It provides an analysis mechanism to monitor the behavior of the users with the help of monitoring tools.
- It’s helpful in microservice architecture to disseminate a single API call to multiple services and compile an answer in return.
- It may provide stabilization to the system by balancing the network traffic.

---

# [API endpoints](#api-endpoints)
It’s imperative to locate the services of microservice architecture in order to acquire their functionality. Therefore, it’s required to define a mechanism for APIs to access the exact location where the service is being provided. We refer to those digital locations as the endpoints of APIs. In a communication channel, the endpoint is one end of a system we can reach with the help of a URL. A user of the service sends a request to the specified endpoint (the URL) to perform operations using the resources available from that endpoint. Usually, the API provider defines a set of endpoints to make the resources available to the users through an HTTP request. The endpoints are also helpful as their names indicate the type of operations they perform (like GET, POST, PUT, and DELETE in case of REST API).

The endpoints are accessed by appending the endpoint name after the base URL of an API. For example, to request information about all the users published on https://jsonplaceholder.typicode.com, the following endpoint is interacted with using an HTTP GET request.

```
HTTP Request - https://jsonplaceholder.typicode.com/users
Base URL - https://jsonplaceholder.typicode.com
Endpoint for getting list of users - /users
```

---
