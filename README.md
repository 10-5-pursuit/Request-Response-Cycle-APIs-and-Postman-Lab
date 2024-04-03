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

> https://amiiboapi.com/

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> Amiibo database (Nintendo Figures) that holds all amiibo information

- What is the URL of the documentation?

> https://amiiboapi.com/docs/

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> nginx/1.15.12

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

```json
{
    "amiibo": [
        {
            "amiiboSeries": "Super Smash Bros.",
            "character": "Cloud Strife",
            "gameSeries": "Final Fantasy",
            "head": "36000000",
            "image": "https://raw.githubusercontent.com/N3evin/AmiiboAPI/master/images/icon_36000000-02590002.png",
            "name": "Cloud",
            "release": {
                "au": "2017-07-22",
                "eu": "2017-07-21",
                "jp": "2017-07-21",
                "na": "2017-07-21"
            },
            "tail": "02590002",
            "type": "Figure"
        },
        {
            "amiiboSeries": "Super Smash Bros.",
            "character": "Cloud Strife",
            "gameSeries": "Final Fantasy",
            "head": "36000100",
            "image": "https://raw.githubusercontent.com/N3evin/AmiiboAPI/master/images/icon_36000100-03620002.png",
            "name": "Cloud - Player 2",
            "release": {
                "au": "2017-07-22",
                "eu": "2017-07-21",
                "jp": "2017-07-21",
                "na": "2017-07-21"
            },
            "tail": "03620002",
            "type": "Figure"
        }
    ]
}

```

- What status code did you get back from your request? Why did you receive this status code?

> 200

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json

> `Content-Length`: 302

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes a complete information about amiibo, including name, series, img, relase date, etc..

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app for collectors, or for people than want to buy a specific amiibo for a specific game

### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> The documentation was simple and clear, it show examples about the data that you can get

- What did you find challenging about the documentation? Cite specific examples.

>  nothing, the documentation is very clear

- Did the quality of the documentation impact your decision to use it?

> Yes, you can find examples very easy

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> Yes, I ended up using the amiibo one, I checked other 3 but the site was very unclear and the documentation was not very useful

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle is the communication between you (your browser) and a server. you make a request to the server and the server respond with some information.

- In your own words, describe what an API is.

> An API is an interface that allows you to get and send information to or from a specific server

- In your own words, describe the purpose of Postman.

> Postman is an application that helps you to visualize and check the status an informations of an api
