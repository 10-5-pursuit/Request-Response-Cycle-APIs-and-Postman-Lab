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

> http://numbersapi.com/

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> The purpose of this API is it give random facts of different numbers in a form of trivia, year, date, or math of whatever that number is.

- What is the URL of the documentation?

> (http://numbersapi.com/)

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> http://numbersapi.com/23/date?json

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

```json
{
 "text": "January 23rd is the day in 1964 that the 24th Amendment to the United States Constitution, prohibiting the use of poll taxes in national elections, is ratified.",
 "year": 1964,
 "number": 23,
 "found": true,
 "type": "date"
}
```

- What status code did you get back from your request? Why did you receive this status code?

> 200

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json; charset=utf-8

> `Content-Length`: 224

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes a random fact about any date of the 23rd in any month.

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app that is a trivia game or intergrate in some type history or math webpage.

### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> The documentation was very easy to read and understand what it does and how to use it. They showed you different usage examples of the API as well like in URL, jquery, etc.

- What did you find challenging about the documentation? Cite specific examples.

> I found the documentation very easy. I didn't have any difficulites figuring out the documentation and how to use the API.

- Did the quality of the documentation impact your decision to use it?

> Yes and No because at first I was hesistant because of how easy the API was to follow but I figured it would be best to start off with something easy first and later on explore more difficult APIs.

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> I stuck with this one.

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle is when the client ask or enter info in the browser or an app, the information is received then sent to the backend to see if it exists, if it does, we send it back to the browser/app, and then send confirmation back to the client.

- In your own words, describe what an API is.

> An API is an application program interface that allows other communication/access points to communicate with other apps.

- In your own words, describe the purpose of Postman.

> Postman is an application that works and manages APIs. It's cleaner version to see how your requests are made, if they're successful, and to see the information requested/sent in a more readable version.
