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

> http://  AnimeChan https://animechan.xyz/

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> The purpose of this API is to allow other clients/Users to  populate a random qoute from a variety of anime with a description of the Qoute, character who spoke it and the anime it was mentioned in. The data provided in this API is objects containing key pair values with an ID number, the qoute it would mention, the anime it's from and character who had said it. I would assume that it is looping randomly through by the ID to autopopulate the qoute in a cycle. I believe any anime fan or aspiring anime watcher would love the use of this API since many inspirational qoutations are said by many characters that we value and pull passion and innovation from. 

- What is the URL of the documentation?

 > meta property="og:url" content="https://animechan.xyz/"

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> https://animechan.xyz/api/random

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

```json
{
    "id": 2556,
    "quote": "It’s hard to forget someone who gave you so much to remember.",
    "anime": "Durarara!!",
    "character": "Izaya Orihara"
}

```

- What status code did you get back from your request? Why did you receive this status code?

> 200: OK. I recieved this code because of a successful HTTP response when I had requested it using GET within POSTMAN. 

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json; charset=utf-8

> `Content-Length`: 134

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes the server that it is coming from and providing a value of what it is. I also noticed that these can be seen as key pair values if we were to view this information another way in JS. It also provides the current connection status and the date in which the request was initiated if it was successful. There are also a list of policies that most likely was generated from the source of it's creation. 

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app that requires an APP NPC in a game that would spit out random qoutes from multiple platforms or if it was on a website for anime and within the homepage it would cycle through anime qoutes from it list of genres/anime hosted on sites similar to CrunchyRoll. 

### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> The documentation was plainly simple and userinterface friendly. I was able to navigate and obtain the information from what it was designed to do. They also have a discord where you can join and promotes further interaction with the community. They also offer a submission option for qoutes that may or may not have been noticed in the documentation that can be added upon request. He also was able to integrate an emoji at the bottom when addressing the creator of the API/documentation.

- What did you find challenging about the documentation? Cite specific examples.

> I found the documentation can be a bit confusing to those who aren't fully aware of JS syntax and may question the display options of the qoutations and not many would be able to understand what to do with the information when traversing through the documentation. 

- Did the quality of the documentation impact your decision to use it?

> Yes because even though it may be confusing to the non developer eye I can utilize it as a source for other projects and integrate my own spin on the design and user interface. 

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> No I ended up sticking with this documentation because I enjoyed deciphering it and understanding how to implement its functionality to get what it is that I wanted from it. 

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle is when you input a request for something from a URL and when the HTTP request is successful it will responde from the server that will generate information or resources from that server. The server will build a response from that request that containes the requested information. 

- In your own words, describe what an API is.

> An API is an application programming interface where it communicates with two or more computer programs so that they can communicate with each other. It's the type of software that takes the requests and delivers it to the server and once the server completes the response returns it back to the origin of request.

- In your own words, describe the purpose of Postman.

> Postman is an application that initiates tests to run requests to ensure that the application pgroamming interface is running smoothly and testing the compability of it's structure and efficiently to deliver the information that's input. you can also view it multiple ways to ensure that that information is accurate the same way that it was coded and intiialized for. 
