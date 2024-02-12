# Simplest REST API in Go

This is a simple REST API in Go. It uses the `net/http` package to create a web server and the `gin-gonic/gin` package to simplify the routing.

The API is a simple record of music albums. It supports the following operations:

- `GET /albums` - Retrieves a list of albums;
- `GET /albums/:id` - Retrieves a specific album;
- `POST /albums` - Creates a new album.

It also has a simples `GET /` route to test the server returning a welcome message. The albums are stored in memory, so if the server is restarted, all data is lost. 

The idea is just to create a simple playground to understand a little bit better Go's sintax and how to create a simple REST API.

## Running the server

To run the server, you need to have Go installed. Then, you can run the following command:

```sh
go run main.go
```

The server will start at `http://localhost:8080`.

## Using the `routes.http` file to test the API

This project has a `routes.http` file that can be used to test the API. It uses the `REST Client` extension for Visual Studio Code. If you have it installed, you can use the `Send Request` link that appears when you hover over the routes in the file.