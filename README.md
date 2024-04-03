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

> [Gutenidex](http://gutenindex.com)

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> The purpose of this API is fetching data from Project Gutenberg Books Library

- What is the URL of the documentation?

> https://gutendex.com/

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> https://gutendex.com/books/55752

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

```json
{
    "id": 55752,
    "title": "Dom Casmurro",
    "authors": [
        {
            "name": "Machado de Assis",
            "birth_year": 1839,
            "death_year": 1908
        }
    ],
    "translators": [],
    "subjects": [
        "Adultery -- Fiction",
        "Authorship -- Fiction",
        "Catholic Church -- Fiction",
        "Reminiscing in old age -- Fiction"
    ],
    "bookshelves": [],
    "languages": [
        "pt"
    ],
    "copyright": false,
    "media_type": "Text",
    "formats": {
        "text/plain; charset=us-ascii": "https://www.gutenberg.org/ebooks/55752.txt.utf-8",
        "text/html": "https://www.gutenberg.org/ebooks/55752.html.images",
        "text/html; charset=iso-8859-1": "https://www.gutenberg.org/files/55752/55752-h/55752-h.htm",
        "application/epub+zip": "https://www.gutenberg.org/ebooks/55752.epub3.images",
        "application/x-mobipocket-ebook": "https://www.gutenberg.org/ebooks/55752.kf8.images",
        "text/plain; charset=iso-8859-1": "https://www.gutenberg.org/files/55752/55752-8.txt",
        "application/rdf+xml": "https://www.gutenberg.org/ebooks/55752.rdf",
        "image/jpeg": "https://www.gutenberg.org/cache/epub/55752/pg55752.cover.medium.jpg",
        "application/octet-stream": "https://www.gutenberg.org/cache/epub/55752/pg55752-h.zip"
    },
    "download_count": 1011
}
```

- What status code did you get back from your request? Why did you receive this status code?

> 200

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json

> `Content-Length`: 1082

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes **title**, **authors**, **subjects**, **copyright**, **formats**, and more.

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app that recoomend books accordingly to the user interests or an app that holds an personal copyright free library.

### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> The documentation was very clear and straight forward. I tryed and selected only books from a certain topic and time period as well as specific languages.

- What did you find challenging about the documentation? Cite specific examples.

> I didn't found anything challenging with the documentation.

- Did the quality of the documentation impact your decision to use it?

> Yes. Not only the documentation was very clear it also linked to resources on how to host my own gutenindex server.

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> I did switch from the API that I initially selected (Corporate Buzz Words) just because it sounded more useful.

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle is summarized by a simple question (or request) sent by the client and a single suitable response sent by the server. 

- In your own words, describe what an API is.

> An API is simply an interface to interact with an external database or service.

- In your own words, describe the purpose of Postman.

> Postman is an application that allow the developer to craft requests and analyse responses (and server behavior).
