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

> http:// The Metropolitan Museum of Art Collection https://metmuseum.github.io/

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> The purpose of this API is to gain access to over 5,000 years of artwork.

- What is the URL of the documentation?

> http://https://metmuseum.github.io/ https://github.com/metmuseum/openaccess.

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> 
https://collectionapi.metmuseum.org/public/collection/v1/objects/45734


- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

```json
{
    "objectID": 45734,
    "isHighlight": false,
    "accessionNumber": "36.100.45",
    "accessionYear": "1936",
    "isPublicDomain": true,
    "primaryImage": "https://images.metmuseum.org/CRDImages/as/original/DP251139.jpg",
    "primaryImageSmall": "https://images.metmuseum.org/CRDImages/as/web-large/DP251139.jpg",
    "additionalImages": [
        "https://images.metmuseum.org/CRDImages/as/original/DP251138.jpg",
        "https://images.metmuseum.org/CRDImages/as/original/DP251120.jpg"
    ],
    "constituents": [
        {
            "constituentID": 11986,
            "role": "Artist",
            "name": "Kiyohara Yukinobu",
            "constituentULAN_URL": "http://vocab.getty.edu/page/ulan/500034433",
            "constituentWikidata_URL": "https://www.wikidata.org/wiki/Q11560527",
            "gender": "Female"
        }
    ],
    "department": "Asian Art",
    "objectName": "Hanging scroll",
    "title": "Quail and Millet",
    "culture": "Japan",
    "period": "Edo period (1615–1868)",
    "dynasty": "",
    "reign": "",
    "portfolio": "",
    "artistRole": "Artist",
    "artistPrefix": "",
    "artistDisplayName": "Kiyohara Yukinobu",
    "artistDisplayBio": "Japanese, 1643–1682",
    "artistSuffix": "",
    "artistAlphaSort": "Kiyohara Yukinobu",
    "artistNationality": "Japanese",
    "artistBeginDate": "1643",
    "artistEndDate": "1682",
    "artistGender": "Female",
    "artistWikidata_URL": "https://www.wikidata.org/wiki/Q11560527",
    "artistULAN_URL": "http://vocab.getty.edu/page/ulan/500034433",
    "objectDate": "late 17th century",
    "objectBeginDate": 1667,
    "objectEndDate": 1682,
    "medium": "Hanging scroll; ink and color on silk",
    "dimensions": "46 5/8 x 18 3/4 in. (118.4 x 47.6 cm)",
    "measurements": [
        {
            "elementName": "Overall",
            "elementDescription": null,
            "elementMeasurements": {
                "Height": 118.4,
                "Width": 47.6
            }
        }
    ],
    "creditLine": "The Howard Mansfield Collection, Purchase, Rogers Fund, 1936",
    "geographyType": "",
    "city": "",
    "state": "",
    "county": "",
    "country": "",
    "region": "",
    "subregion": "",
    "locale": "",
    "locus": "",
    "excavation": "",
    "river": "",
    "classification": "Paintings",
    "rightsAndReproduction": "",
    "linkResource": "",
    "metadataDate": "2020-09-14T12:26:37.48Z",
    "repository": "Metropolitan Museum of Art, New York, NY",
    "objectURL": "https://www.metmuseum.org/art/collection/search/45734",
    "tags": [
        {
            "term": "Birds",
            "AAT_URL": "http://vocab.getty.edu/page/aat/300266506",
            "Wikidata_URL": "https://www.wikidata.org/wiki/Q5113"
        }
    ],
    "objectWikidata_URL": "https://www.wikidata.org/wiki/Q29910832",
    "isTimelineWork": false,
    "GalleryNumber": ""
}

```

- What status code did you get back from your request? Why did you receive this status code?

> Status recieved 200 OK. I recieved this status beacause the request was valid and correlated to the specific id of that object.

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json; charset=UTF-8

> `Content-Length`: Not provided.

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes details of a painting called Quail and Millet designed by a female artist named Kiyohara Yukinob, from the the Japanese culture. Details include dimensions of the painting the period in which was the painting was started and ended. Full description of the artist and the painting's design.

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app that is affiliated with ancient Japanese art, that can be accessed by title, era and illustrator.
> I could imagine integrating this API into an app dedicated to showcasing art from a specific era or period in history.


### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> The documentation was very informative about the Museum of Art and the type of artwork that is presented at the museum over 470,000 artworks in it's collection for unrestricted commercial and noncommercial use. 

- What did you find challenging about the documentation? Cite specific examples.

> I found the documentation was very clear, and well presented, I have no complaints.

- Did the quality of the documentation impact your decision to use it?

> Yes because it was the comprehensive documention I encountered while looking for other API's to use. 

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> Yes I ended up switching and using this API over CityBikes API https://api.citybik.es/v2/ beacuse I felt that this documentation had very little explaination was clear, but short not very descriptive.

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle is when A user / client requests information and response is the data being rendered from a server and returened to the user.

- In your own words, describe what an API is.

> An API is Application Programming Interface is what software applications use to communicate with each other.  

- In your own words, describe the purpose of Postman.

> Postman is an application that makes working with API's more manageable, easier to understand and comprehend. Postman focuses on testing API's which helps improve development process.
