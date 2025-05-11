# [Introduction to APIs](#introduction-to-apis)

## [What is an Application Programming Interface?](#what-is-an-application-programming-interface)
An application programming interface (API) is an intermediary through which two software components communicate to share data and to get useful work done. As the name implies, exchanging information is possible because of the presence of a software interface between these components. The software components can reside on the same or different machines connected through a network.

Using an API, an application can request services from another application without understanding the architecture of other applications. The only thing the requesting application should know is how to place the request, in other words, it should understand the interface for placing the request.

---

# [Benefits of APIs](#benefits-of-apis)
Some major advantages of using APIs are as follows:

* **Complexity abstraction:** New services are often complex, with many moving parts. APIs help us to hide all that complexity within a service away from the consumer. Doing so has many benefits, such as the flexibility to change the internals of the service without changing the interface. With APIs, the caller of the service can focus on their application without worrying about the internal complexity of the calling service. The caller only has to focus on the interface and return data from the callee.

* **Improved modularity:** APIs aid the microservices architecture of applications by further breaking down applications into subsets of services. Developers use this modularity to design a flexible, maintainable, and reusable application.

* **Efficient development:** APIs have reduced the development time and the number of bugs by preventing developers from having to rewrite code for the same functionality. With APIs, developers can request services by making a simple call, without the need to rewrite code from scratch.

* **API expedites digitization:** APIs were critical for expedited digitization, especially since the start COVID-19. According to the Moesif summary of a McKinsey report: "Coronavirus has acted as an accelerant on companies offering digital products and services. Across all business areas, digital adoption has accelerated to such a degree that it’s the equivalent of fast-forwarding six years where 60% of all businesses in the US employ digital processes".

* **Controlled accessibility:** APIs provide applications with the flexibility to share limited data or information with a restricted number of users. Other techniques can be used to throttle the frequency of service usage.

---

# [Types of APIs](#types-of-apis)
The APIs can be divided into four types based on users and their access levels, as shown below:

- **Public APIs** are intended for developers to access publicly available data or services. Public APIs are freely accessible, but are limited to a few calls for a certain time period.

- **Private APIs** are designed for internal use only. The developers working within the company can use them to improve their products and services. They have the highest level of access and can see and update the complexity of the back-end system.

- **Partner APIs** are for users that have business relationships with the company that owns the APIs. These APIs have more robust security measures than public APIs. Generally, they are purpose-specific—such as giving access to a prepaid service—and are a widely used pattern in the ecosystem.

- **Composite APIs** allow developers to bundle the request call for different services and get a unified response from different requested resources. Composite APIs are handy when a developer needs data from different servers without making a separate API call to each server. It makes the system work faster and more efficiently by reducing the number of API calls and complexity.

---

