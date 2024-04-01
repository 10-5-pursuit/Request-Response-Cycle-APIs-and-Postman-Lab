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
> https://metmuseum.github.io/

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> The purpose of this API is...
> To provide developers with hundreds upon thousands of artwork in the public domain for use for unrestricted commercial and noncommercial use.

- What is the URL of the documentation?

> https://github.com/metmuseum/openaccess

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

> https://collectionapi.metmuseum.org/public/collection/v1/objects/437133

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

```json
{
"objectID": 437133,
"isHighlight": true,
"accessionNumber": "67.241",
"accessionYear": "1967",
"isPublicDomain": false,
"primaryImage": "",
"primaryImageSmall": "",
"additionalImages": [],
"constituents": [
{
"constituentID": 162135,
"role": "Artist",
"name": "Claude Monet",
"constituentULAN_URL": "http://vocab.getty.edu/page/ulan/500019484",
"constituentWikidata_URL": "https://www.wikidata.org/wiki/Q296",
"gender": ""
}
],
"department": "European Paintings",
"objectName": "Painting",
"title": "Garden at Sainte-Adresse",
"culture": "",
"period": "",
"dynasty": "",
"reign": "",
"portfolio": "",
"artistRole": "Artist",
"artistPrefix": "",
"artistDisplayName": "Claude Monet",
"artistDisplayBio": "French, Paris 1840–1926 Giverny",
"artistSuffix": "",
"artistAlphaSort": "Monet, Claude",
"artistNationality": "French",
"artistBeginDate": "1840",
"artistEndDate": "1926",
"artistGender": "",
"artistWikidata_URL": "https://www.wikidata.org/wiki/Q296",
"artistULAN_URL": "http://vocab.getty.edu/page/ulan/500019484",
"objectDate": "1867",
"objectBeginDate": 1867,
"objectEndDate": 1867,
"medium": "Oil on canvas",
"dimensions": "38 5/8 x 51 1/8 in. (98.1 x 129.9 cm)",
"measurements": [
{
"elementName": "Overall",
"elementDescription": null,
"elementMeasurements": {
"Height": 98.1,
"Width": 129.9
}
},
{
"elementName": "Frame",
"elementDescription": null,
"elementMeasurements": {
"Depth": 12.7,
"Height": 133.3503,
"Width": 166.3703
}
}
],
"creditLine": "Purchase, special contributions and funds given or bequeathed by friends of the Museum, 1967",
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
"metadataDate": "2024-01-13T04:57:36.57Z",
"repository": "Metropolitan Museum of Art, New York, NY",
"objectURL": "https://www.metmuseum.org/art/collection/search/437133",
"tags": [
{
"term": "Gardens",
"AAT_URL": "http://vocab.getty.edu/page/aat/300008090",
"Wikidata_URL": "https://www.wikidata.org/wiki/Q1107656"
},
{
"term": "Men",
"AAT_URL": "http://vocab.getty.edu/page/aat/300025928",
"Wikidata_URL": "https://www.wikidata.org/wiki/Q8441"
},
{
"term": "Women",
"AAT_URL": "http://vocab.getty.edu/page/aat/300025943",
"Wikidata_URL": "https://www.wikidata.org/wiki/Q467"
},
{
"term": "Seas",
"AAT_URL": "http://vocab.getty.edu/page/aat/300008694",
"Wikidata_URL": "https://www.wikidata.org/wiki/Q165"
},
{
"term": "Boats",
"AAT_URL": "http://vocab.getty.edu/page/aat/300178749",
"Wikidata_URL": "https://www.wikidata.org/wiki/Q35872"
}
],
"objectWikidata_URL": "https://www.wikidata.org/wiki/Q432253",
"isTimelineWork": true,
"GalleryNumber": "818"
}

```

- What status code did you get back from your request? Why did you receive this status code?

> 200 OK because the request was valid and there was a corresponding id in the database

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json; charset=UTF-8

> `Content-Length`: not listed

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes...
> This is a the data on the piece "Garden at Sainte-Adresse" by Claude Monet. The piece was acquired in 1967 and noted as an important piece of artwork that is not in the public domain. It also includes information on the artist such that Monet was a french artist born in the year 1840 and died the year 1926.

- Identify at least two ways to use the data within a web application.

> I could imagine integrating this API into an app that ...Can identify an piece of artwork by either it's title or the artists title to provide a summary about the artists background.

### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> The documentation was ... concise in its ability to highlight their names used for objects in the JSON and explaining what the data represented.

- What did you find challenging about the documentation? Cite specific examples.

> I found the documentation ...inaccurate in its example as the id provided led to a Claude Monet piece when the example suggests it to be a work by Van Gogh. It was also difficult finding an ID i might want on a particular piece without guessing.

- Did the quality of the documentation impact your decision to use it?

> Yes/No because... Yes because I was about to access the data I needed for the project though it was not my first choice

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> Yes/No I ended up ... I did not choose based on its documentation but switched APIs based on the level of access and ease of use

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle ... similar to a call and response. The user inputs a call using the browser to its appropriate server, which then responds back with its appropriate response, making its own call & response to the database if necessary.

- In your own words, describe what an API is.

> An API is ... A collection of data typically in JSON format that can be used repeatedly for various projects.

- In your own words, describe the purpose of Postman.

> Postman is an application that ... Allows developers to make calls and get additional data on the request response cycle as well as look at the results of the response to analyze the API.