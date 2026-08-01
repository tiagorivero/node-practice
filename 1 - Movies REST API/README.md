# Movies REST API

A REST API built with Node.js and Express to practice CRUD operations, data validation, and CORS configuration.

## Features

- Get all movies, or filter by genre
- Get a single movie by ID
- Create a new movie (with full validation)
- Update a movie partially (PATCH)
- Delete a movie
- Request/response validation using Zod schemas
- CORS configured with an explicit list of allowed origins
- Includes a simple HTML client to fetch and delete movies from the browser

## Tech stack

- Node.js
- Express
- Zod
- CORS

## Backend concepts practiced

- Building a RESTful API (GET, POST, PATCH, DELETE)
- Route params and query strings
- Schema validation with Zod (`safeParse`, `.partial()`)
- CORS configuration and allowed origins
- Generating unique IDs with `crypto.randomUUID()`

## Run locally

Clone the repository and install the dependencies:

```bash
npm install
```

Start the server:

```bash
node index.js
```

The server runs on `http://localhost:1234` by default. You can test the endpoints using the included `.http` file (with the REST Client extension in VS Code) or by opening `index.html` in your browser.