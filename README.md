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

> The Metropolitan Museum of Art Collection API  https://metmuseum.github.io/

- What is the purpose of this API? Describe what data the API provides and why someone might want to use it.

> The Metropolitian museum API is used to gain public access to all works of art, displayed or archived within the museum through the web.

- What is the URL of the documentation?

> https://metmuseum.github.io/

### Response

For the following questions, choose a single endpoint to request within Postman.

- What is the full URL of the endpoint?

https://collectionapi.metmuseum.org/public/collection/v1/objects/437133

- What response do you receive when you make a request to that endpoint? Be sure to wrap your answer in the correct formatting for JSON.

```json

   {"objectID":437133,"isHighlight":true,"accessionNumber":"67.241","accessionYear":"1967","isPublicDomain":false,"primaryImage":"","primaryImageSmall":"","additionalImages":[],"constituents":[{"constituentID":162135,"role":"Artist","name":"Claude Monet","constituentULAN_URL":"http://vocab.getty.edu/page/ulan/500019484","constituentWikidata_URL":"https://www.wikidata.org/wiki/Q296","gender":""}],"department":"European Paintings","objectName":"Painting","title":"Garden at Sainte-Adresse","culture":"","period":"","dynasty":"","reign":"","portfolio":"","artistRole":"Artist","artistPrefix":"","artistDisplayName":"Claude Monet","artistDisplayBio":"French, Paris 1840–1926 Giverny","artistSuffix":"","artistAlphaSort":"Monet, Claude","artistNationality":"French","artistBeginDate":"1840","artistEndDate":"1926","artistGender":"","artistWikidata_URL":"https://www.wikidata.org/wiki/Q296","artistULAN_URL":"http://vocab.getty.edu/page/ulan/500019484","objectDate":"1867","objectBeginDate":1867,"objectEndDate":1867,"medium":"Oil on canvas","dimensions":"38 5/8 x 51 1/8 in. (98.1 x 129.9 cm)","measurements":[{"elementName":"Overall","elementDescription":null,"elementMeasurements":{"Height":98.1,"Width":129.9}},{"elementName":"Frame","elementDescription":null,"elementMeasurements":{"Depth":12.7,"Height":133.3503,"Width":166.3703}}],"creditLine":"Purchase, special contributions and funds given or bequeathed by friends of the Museum, 1967","geographyType":"","city":"","state":"","county":"","country":"","region":"","subregion":"","locale":"","locus":"","excavation":"","river":"","classification":"Paintings","rightsAndReproduction":"","linkResource":"","metadataDate":"2024-01-13T04:57:36.57Z","repository":"Metropolitan Museum of Art, New York, NY","objectURL":"https://www.metmuseum.org/art/collection/search/437133","tags":[{"term":"Gardens","AAT_URL":"http://vocab.getty.edu/page/aat/300008090","Wikidata_URL":"https://www.wikidata.org/wiki/Q1107656"},{"term":"Men","AAT_URL":"http://vocab.getty.edu/page/aat/300025928","Wikidata_URL":"https://www.wikidata.org/wiki/Q8441"},{"term":"Women","AAT_URL":"http://vocab.getty.edu/page/aat/300025943","Wikidata_URL":"https://www.wikidata.org/wiki/Q467"},{"term":"Seas","AAT_URL":"http://vocab.getty.edu/page/aat/300008694","Wikidata_URL":"https://www.wikidata.org/wiki/Q165"},{"term":"Boats","AAT_URL":"http://vocab.getty.edu/page/aat/300178749","Wikidata_URL":"https://www.wikidata.org/wiki/Q35872"}],"objectWikidata_URL":"https://www.wikidata.org/wiki/Q432253","isTimelineWork":true,"GalleryNumber":"818"}

```

- What status code did you get back from your request? Why did you receive this status code?

> 200 OK

- Click on the **response** headers in Postman. What are the `Content-Type` and `Content-Length` (provide exact values)?

> `Content-Type`: application/json; charset=UTF-8

> `Content-Length`: I see no information on content-length, within the header.

- Summarize the most salient parts of the data you are getting back. How would you describe what is included within the response?

> The data we received includes JSON arrays, and objects, listing data on the artist, such as name, age, birth.  And the rest are information on the specified work of art, such as the building material, medium, and location/time/country in which the artwork was built.

- Identify at least two ways to use the data within a web application.

> You can use the data to query historic artifact images for learning purposes inside of a web app.
>  You can also use the MET API in order to gain brief biographical information into the artist, and the countries and cultures which they lived.

### Documentation

The following questions relate to the documentation of the API.

- What did you like about the documentation? Cite specific examples.

> I enjoyed the very purpose of the API, which is to query images and various information about all of the art works presented in the metropolitan museum.  I like the way the document instructs you to query for various objects and collections of information with their API.


- What did you find challenging about the documentation? Cite specific examples.

> Over all, I find it hard to differentiate what a GET and a Response is, other than the fact that a response, adds a header and status information regarding the connection of the data with the API.

- Did the quality of the documentation impact your decision to use it?

> This specific documentation made APIs more interesting to me. I did not understand the structure of URL browser quering until I read the documentation.  And I look forward to experementing with this API in order to strengthen my experience and understanding with APIs.

- Did you switch which API you chose initially because of its documentation, or did you stick with the one you selected and work your way through it?

> Actually this Metropolitan Museum API is the first and only API documentation I bothered reading and experimenting with. This is also because I generally enjoy going to the MET museum.  So it's fascinating to learn about APIs and the items that are currated in the museum, using this API.

### Definitions

The following questions require you to define some concepts and terms. Provide detailed explanations.

- In your own words, summarize the request-response cycle.

> The request-response cycle are rules and protocols that must take place when an API is communicating with a server and/or client.  The API must request data in various forms, depending on the file path of the URL.  When a request is sent, the query is pending, and when the request is completed, the response is satisfied with a code number: 200.  If the code does not respond correctly, you will either recieve a 404 number, which indicates a missing document, or connection loss.  Or a 500, number, which indicates a server problem.

- In your own words, describe what an API is.

> An API controls what type of data a client can recieve or send.  The API can also control the amounts of data that can be transfered to and fro.  The API is the messenger between the client and the server where all of the data is being stored in.  

- In your own words, describe the purpose of Postman.

> Postman seems to be used to help developers create, model and test their own APIs for effeciency, as well as 3rd party APIs that you may encounter on the internet.
