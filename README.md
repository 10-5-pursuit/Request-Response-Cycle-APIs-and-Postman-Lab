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

> 
An API of Ice And Fire
http://anapioficeandfire.com/

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> The purpose of this API is to offer structured data from the Ice And Fire books and the Game of Thrones series, covering characters, houses, books, and more. It's designed for fans and developers looking to build applications or perform analyses on this universe, providing detailed series-related information.

- What is the URL of the documentation?

> https://anapioficeandfire.com/api/

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> https://anapioficeandfire.com/api/houses/350

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

```json

{
    "url": "https://anapioficeandfire.com/api/houses/350",
    "name": "House Shett of Gull Tower",
    "region": "The Vale",
    "coatOfArms": "Three golden wings, bendwise, on a checkered white and black field(Chequy argent and sable, in bend three dexter wings elevated bendwise or)",
    "words": "",
    "titles": [
        "the Knight of Gull Tower"
    ],
    "seats": [
        "Gull Tower"
    ],
    "currentLord": "https://anapioficeandfire.com/api/characters/287",
    "heir": "",
    "overlord": "https://anapioficeandfire.com/api/houses/328",
    "founded": "",
    "founder": "",
    "diedOut": "",
    "ancestralWeapons": [],
    "cadetBranches": [],
    "swornMembers": [
        "https://anapioficeandfire.com/api/characters/287"
    ]
}

```

- What status code did you get back from your request? Why did you receive this status code?

> 200 OK because the request was valid and there was a corresponding id in the database

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json; charset=utf-8

> `Content-Length`: not listed

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes "House Shett of Gull Tower" which is found in the Vale region. It's coat of arms consists of three golden wings, bendwise, on a checkered white and black field.

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app that needs to create a card for house vassals that serve the main houses of Westeros.

### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> The documentation was simple and legible. 

- What did you find challenging about the documentation? Cite specific examples.

> I didn't find any challenges. 

- Did the quality of the documentation impact your decision to use it?

> Yes because it was easier to read through compared to the other APIs I tried to test.

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> Yes I switched with other APIS because of how complex and difficult they were to read.

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle is when the first computer sends a request for certain data and the second computer responds to the requests. 

- In your own words, describe what an API is.

> An API is a mechanism that enables 2 software components to communicate with each other using a set of definitions and protocols. 

- In your own words, describe the purpose of Postman.

> Postman is an application that helps share, test and document APIs.
