# Node.js RESTful API Example

1.  Install Dependencies

    * [Node.js (version 6.x is recommended)](https://nodejs.org/en/)

3.  Go to the project's root directory **cd /my/path/to/directory**
4.  Run **npm install**
5.  Start using it! **npm start**

## Available end-points

### GET /events

Gets all the available events (12 sample events).

### GET /events/:id

Obtains an event given its id.

### POST /events

Creates an event (be sure you are sending the headers via your library).

**Headers**

Content-Type : application/json

**Request body (raw)**

```
    {
        "topics": "",
        "thumbnail": "/img/tr-3.jpeg",
        "url": "index.html",
        "overrideURL": "",
        "linkType": "",
        "title": "Created by Postman",
        "summary": "Lorem ipsum dolor sit amet"
    }
```

### PUT /events/:id

Updates an existing event. The JSON object must be passed in the request body as raw. It returns an error in case the event doesn't exist.

**Headers**

Content-Type : application/json

**Request body (raw)**

```
    {
        "id": "1",
        "topics": "",
        "thumbnail": "/img/tr-3.jpeg",
        "url": "index.html",
        "overrideURL": "",
        "linkType": "",
        "title": "Updated by Postman",
        "summary": "Lorem ipsum dolor sit amet"
    }
```

### DELETE /events/:id

Removes an event given its id.




