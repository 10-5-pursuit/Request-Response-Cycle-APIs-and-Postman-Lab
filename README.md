# Request Response Cycle, APIs, and Postman Lab

You will be working with a free API of your choice for this lab.

## Getting Started

1. Choose an API with no auth and no CORS from the following list. It _should not_ be one that you've already seen or worked on in class.
   - [Public APIs](https://github.com/public-apis/public-apis)
2. Choose an API not covered in your readings, class, or other assignments. The API should be new to you.
3. Write your answers in this README.md file. Do not delete the questions. Write your answers after the `>`. If you need to write more than one paragraph, add more `>`.
4. Take the time to read back the work, and edit what you've written so that your answers are clear and anyone reading it can easily understand what you've written.

## Instructions

Do your best to answer the questions with specific details. Writing about code clearly and thoroughly is a critical skill to practice.

- Which one did you choose? Provide the name and base URL.

> https://getpantry.cloud/

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> The purpose of this API is...Pantry is a free data storage service which allows users to manage a collection of JSON objects. It is great for small to medium sized projects, and can be interacted with through a RESTful API or via a dashboard.

- What is the URL of the documentation?

> https://documenter.getpostman.com/view/3281832/SzmZeMLC

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> https://getpantry.cloud/apiv1/pantry/<YOUR_ID>/basket/<BASKET_NAME>

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

{
  "message": "Unauthorized"
}


- What status code did you get back from your request? Why did you receive this status code?

> I received a status code of 401 (Unauthorized). This shows that my request did not have proper authentication or authorization credentials to access the endpoint.

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json

> `Content-Length`: 28

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes a JSON object with a single key-value pair, the key is "message" and the value is "Unauthorized". This indicates that the request was unsuccessful due to lack of proper authorization.

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app that would need a small dbase to hold information for display.

### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> I appreciated the clarity of the endpoints and the provided examples in the documentation. For instance, the examples given for each endpoint helped in understanding how to structure requests properly.

- What did you find challenging about the documentation? Cite specific examples.

> One challenge I found was the lack of detailed information regarding authentication and authorization requirements for accessing the endpoints. It would have been helpful to have clearer instructions or links to additional resources on this topic.

- Did the quality of the documentation impact your decision to use it?

> Yes, to some extent. While the documentation was generally clear, the lack of detailed information on authentication raised concerns about the ease of integrating the API into my project.

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> No, I stuck with the Pantry API and worked my way through the documentation to understand its capabilities and how to interact with it effectively.

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle is a fundamental concept in web development that describes the flow of communication between a client (such as a web browser or a mobile app) and a server. It begins with the client sending a request to the server, which includes information about the desired action (e.g., fetching data, submitting a form). The server then processes the request and generates a response, which is sent back to the client. The response typically contains the requested data or indicates the outcome of the requested action.

- In your own words, describe what an API is.

> An API (Application Programming Interface) is a set of rules and protocols that allows different software applications to communicate and interact with each other. It defines the methods and data formats that applications can use to request and exchange information. APIs enable developers to build upon existing functionality or services provided by other applications without needing to understand their internal workings, making it easier to create complex systems by leveraging the capabilities of multiple software components.

- In your own words, describe the purpose of Postman.

> Postman is an application that simplifies the process of testing, documenting, and interacting with APIs. It provides a user-friendly interface for sending HTTP requests to API endpoints, allowing developers to easily explore and experiment with different API functionalities. Postman also enables the creation of automated tests and the generation of comprehensive API documentation, streamlining the development and debugging process for API-driven applications.
