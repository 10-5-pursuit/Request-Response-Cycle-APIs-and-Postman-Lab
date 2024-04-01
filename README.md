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

> https://api.disneyapi.dev/

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> The purpose of this API is to privide information on the massive catalogue of disney characters and their many ttributes such as name, films, tv shows, allies, enemies, etc.

- What is the URL of the documentation?

> https://api.disneyapi.dev/character

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> https://api.disneyapi.dev/characters/4703

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

```json
{
    "info": {
        "count": 1,
        "totalPages": 1,
        "previousPage": null,
        "nextPage": null
    },
    "data": {
        "_id": 4703,
        "films": [
            "Hollywood Party",
            "Fantasia",
            "Fun and Fancy Free",
            "TRON",
            "Who Framed Roger Rabbit",
            "Oliver & Company",
            "The Little Mermaid",
            "Toy Story",
            "A Goofy Movie",
            "Mickey's Once Upon a Christmas",
            "Fantasia 2000",
            "Mickey's Magical Christmas: Snowed in at the House of Mouse",
            "Mickey's House of Villains",
            "Teacher's Pet (film)",
            "The Lion King 1½",
            "101 Dalmatians II: Patch's London Adventure",
            "Mickey, Donald, Goofy: The Three Musketeers",
            "Mickey's Twice Upon a Christmas",
            "Chicken Little (film)",
            "Meet the Robinsons",
            "Wreck-It Ralph (film)",
            "Saving Mr. Banks",
            "Frozen",
            "Zootopia",
            "Ralph Breaks the Internet"
        ],
        "shortFilms": [],
        "tvShows": [
            "Walt Disney anthology series",
            "The Mickey Mouse Club",
            "The Mouse Factory",
            "Adventures of the Gummi Bears",
            "Bonkers",
            "101 Dalmatians: The Series",
            "Mickey Mouse Works",
            "House of Mouse",
            "Mickey Mouse Clubhouse",
            "Imagination Movers",
            "Mickey's Letter Time",
            "Have a Laugh!",
            "Mickey’s Mousekersize",
            "A Poem Is...",
            "Mickey Mouse (TV series)",
            "Minnie's Bow-Toons",
            "Once Upon a Time",
            "Frozen: Northern Lights",
            "At Home With Olaf",
            "Mickey Mouse Mixed-Up Adventures",
            "DuckTales (2017 series)",
            "Mickey Go Local",
            "The Wonderful World of Mickey Mouse",
            "WandaVision",
            "Mickey Mouse Funhouse"
        ],
        "videoGames": [
            "Mickey Mouse: The Computer Game",
            "Mickey Mousecapade",
            "Adventures in the Magic Kingdom",
            "Illusion (series)",
            "The Magical Quest starring Mickey Mouse",
            "Mickey Mania: The Timeless Adventures of Mickey Mouse",
            "Mickey's Speedway USA",
            "Mickey's Racing Adventure",
            "Disney's Party",
            "Disney's Magical Mirror Starring Mickey Mouse",
            "Disney's Hide and Sneak",
            "Disney Friends",
            "Kingdom Hearts (series)",
            "Epic Mickey (series)",
            "Kinect Disneyland Adventures",
            "Disney Infinity (series)",
            "Disney Magical World",
            "Disney Magical World 2",
            "Where's My Mickey?",
            "Disney Tsum Tsum (game)",
            "Disney Magical Dice",
            "Disney Heroes: Battle Mode",
            "Disney Mirrorverse",
            "Disney Sorcerer's Arena"
        ],
        "parkAttractions": [
            "Mickey and Minnie's Runaway Railway",
            "Fantasmic!",
            "Mickey's PhilharMagic",
            "Mickey's Royal Friendship Faire",
            "World of Color",
            "Main Street Electrical Parade",
            "Mickey Mouse Revue",
            "Town Square Theater",
            "Mickey's House and Meet Mickey",
            "One Man's Dream II: The Magic Lives On!",
            "Midship Detective Agency",
            "My Friend Duffy",
            "The Golden Mickeys",
            "Festival of Fantasy Parade",
            "Paint the Night Parade",
            "Mickey and the Magical Map",
            "Wonderful World of Animation"
        ],
        "allies": [],
        "enemies": [],
        "sourceUrl": "https://disney.fandom.com/wiki/Mickey_Mouse",
        "name": "Mickey Mouse",
        "imageUrl": "https://static.wikia.nocookie.net/disney/images/9/99/Mickey_Mouse_Disney_3.jpeg",
        "createdAt": "2021-04-12T02:33:01.829Z",
        "updatedAt": "2021-12-20T20:40:04.583Z",
        "url": "https://api.disneyapi.dev/characters/4703",
        "__v": 0
    }
}

```

- What status code did you get back from your request? Why did you receive this status code?

> 200  
> This indicates a successful request

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json; charset=utf-8

> `Content-Length`: 2795

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes the name, tv shows, video games, an image url, and the films that applies to this specific character

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app that aloows users to identify whether or not a set of characters appear in the same media, or an app that allows users to tell whether or not their are specific theme park attractions revolved around a specific character

### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> The documentation was clear, concise and easy to follow. The URL needed to extract a specific character or a set of characrters w/ identical key/value pairs was easily identifiable

- What did you find challenging about the documentation? Cite specific examples.

> I found the documentation a little confusing when it mentions GraphQL. I've never heard of that before

- Did the quality of the documentation impact your decision to use it?

> Yes because the way it was written made it easy to understand the data and extract specifc entries

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> No, I ended up sticking with the first one I found. I got lucky with the disney api. The data is also very straight-forward.

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle is when you/your computer(the client) requests information or an action to be performed on a server(the host) and from that request the server then sends a requests indicating whether it was succesful, unsuccesful, or somewhere in-between.

- In your own words, describe what an API is.

> An API is a set of data that is hosted somewhere like a server, to be accessed by app developers to make their projects more feature rich or privide more information to an end user.

- In your own words, describe the purpose of Postman.

> Postman is an application that allows devs to Create, Read, Update, or Delete the data in an api in a way that allows for the testing of endpoints and viewing raw data in a more user friendly way
