# [Deep dive into API Design Concepts](#deep-dive-into-api-design-concepts)

## [What is API design?](#what-is-api-design)
API design is carefully planning, preparing, and developing programming interfaces (APIs) to expose data and the system’s functionality to consumers. APIs enable system-to-system communication and are essential for digital organizations because they add new capabilities to their products, operations, partnership strategies, and more. An effective API design is one that has satisfactory answers to the following queries of a developer:

Why is the API being developed?
- What would be the outcome regarding the impact and output of the system?
- How will the API be designed to meet the requirements?
- What will be the structure of our resources?
- How will we document our resources?

---

## [API design considerations](#api-design-considerations)
The following illustration shows the key points for better API design:
![image](https://github.com/user-attachments/assets/daf0e7ef-07a1-49e1-a2fa-cb61a33292dc)
- Identify the potential users in terms of their relationship with the business (partners, customers, or external developers) for which API is being developed. This identification will define the level of access and type of authentication to be implemented in the API. The types of users will also help identify and implement the correct architectural style, REST, gRPC, and so on.
- Identify what developer problems are being solved in terms of their business relationship, critical needs, and value addition. Identifying the metrics that will improve after using the developed API is also necessary. These metrics include revenue, task speed, cost, and so on.
- It is important to identify the responses (successes or errors) to different API calls so that developers can understand the type and reason of the responses received from the server. Exception and error handling must be implemented along with well-defined endpoints of the API.
- Real-life use-case implementation should be applied so that the testability factor is checked and developers can understand the effectiveness of the designed API in terms of challenges and opportunities. While designing, we should analyze the performance of the API by testing different possible use cases.
- The API should be scalable to handle the increasing demands of customers. Therefore, the API’s design should consider scalability as an important factor in order to avoid fundamental modifications in the future.
- The API should be adequately documented so the developers can easily understand the integration, behaviors, structures, and parameters to be defined while using the API.

---

## [API requirements](#api-requirements)
We need to define both the functional and non-functional requirements of our APIs. Take a look at both the requirements types below:
- **Functional requirements** define the desired end function of a system and its required parameters. For example, in a video streaming service, the ability to post comments on a video is a functional requirement because it has a defined end goal and parameters.
- **Non-functional requirements** define the performance and quality of the services the API provides. Continuing from the video streaming example above, the ability of an API to quickly respond to the user (low latency) or a number of users posting comments simultaneously (scalability) are forms of non-functional requirements. Other non-functional requirements include availability, reliability, consistency, and so on.
  
![image](https://github.com/user-attachments/assets/67c6631c-45ae-4d5c-9798-89755cb0459a)

## [Characteristics of a Good API Design](#characteristics-of-a-good-api-design)

| Characteristic                                      | Explanation                                                                                                                                                       |
|----------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Separation between API specification and its implementation | Includes separation between the specification and its implementation, allowing for iterative improvements and changes to the API implementation.                  |
| Concurrency                                         | Amount of API calls that can be active simultaneously in a specified period, ensuring that computing resources are available for all users.                     |
| Dynamic rate-limiting                               | Strategy to limit access to the API within a timeframe to avoid overwhelming the API with an onslaught of requests.                                              |
| Security                                            | Well-defined security mechanisms for authentication and authorization protocols that define who can access the API and what parts of the API they can access.  |
| Error warnings and handling                         | Allows effective error handling to prevent frustration on the consumer end and reduces debugging efforts for developers.                                         |
| Architectural styles of an API                     | Possible to follow different architectural styles according to its requirements.                                                                                 |
| Minimal but comprehensive and cohesive              | API should be as terse as possible while still fulfilling its goals.                                                                                            |
| Stateless or state-bearing                          | API functions can be stateless and/or maintain their state, but idempotency (operations yielding the same result when performed multiple times) is a desired feature. |
| User adoption                                       | APIs with good adoption often have a devoted user community that helps improve the API over many iterations.                                                     |
| Fault tolerance                                     | A well-designed API can be made fault-tolerant by using mechanisms that ensure continued operation, even if some components malfunction.                         |
| Performance measurement                             | There should be appropriate provisions for collecting monitoring data and early warning systems.                                                                  |

---
