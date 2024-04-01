# Request Response Cycle, APIs, and Postman Lab

You will be working with a free API of your choice for this lab.

## Getting Started

1. Choose an API with no auth and no CORS from the following list. It _should not_ be one that you've already seen or worked on in class.
   - [Public APIs](https://github.com/public-apis/public-apis)
1. Choose an API not covered in your readings, class, or other assignments. The API should be new to you.
1. Write your answers in this README.md file. Do not delete the questions. Write your answers after the `>`. If you need to write more than one paragraph, add more `>`.
1. Take the time to read back the work, and edit what you've written so that your answers are clear and anyone reading it can easily understand what you've written.

## Instructions

Do your best to answer the questions with specific details. Writing about code clearly and thoroughly is a critical skill to practice.

- Which one did you choose? Provide the name and base URL.

> The Metropolitan Museum of Art Collection API

> http://metmuseum.github.io/

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> The purpose of this API is to provide information about certain collections, so it could be use for media.

- What is the URL of the documentation?

> http://metmuseum.github.io/

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> http://collectionapi.metmuseum.org/public/collection/v1/objects

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

JSON

```
{
    "total": 487735,
    "objectIDs": [
        1,
        2,
        3,
        4,
        5,
        6,
        7,
        8,
        9,
        10,
        ...more
   ]
}
```

- What status code did you get back from your request? Why did you receive this status code?

> 200, request was succesful

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json; charset=UTF-8

> `Content-Length`: N/A

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes an object with a total key, which is how big the data set is, and the objectIDs key, which is an array with all ids

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app that wants to make a guide for tourists on what to visit in MET. Another way it could be use, is if you wanna make like a trivia game.

### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> The documentation was really straight forward with the explanations and good examples on how to use it.

- What did you find challenging about the documentation? Cite specific examples.

> I think this API was well documented and explained everything fairly clear

- Did the quality of the documentation impact your decision to use it?

> I don't see a reason where I would use it personally, but I think it's helpful depending on what you're doing with it.

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> I switched because their documentaion was really vague.

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle is the communication between client and server, and how each request prmpts a response and vice versa.

- In your own words, describe what an API is.

> An API is a way for others to work with a certain data set

- In your own words, describe the purpose of Postman.

> Postman is an application that allows us to see everything that happens with a HTTPS request
