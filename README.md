# Go CRUD Movies API

This project demonstrates a simple CRUD (Create, Read, Update, Delete) movies API built in Go. Instead of using a database, it utilizes structs and slices to manage data, providing a solid foundation for understanding Go's native data structures and their manipulation.

## Overview

- **Tech Stack**: Go, Gorilla Mux
- **Purpose**: Learn Go structs, slices, and basic HTTP handling.
- **Features**:
  - Create a movie
  - Read (get) all movies
  - Read (get) a single movie by ID
  - Update a movie by ID
  - Delete a movie by ID

## Running the Server

1. Clone the repository.
2. Navigate to the project directory.
3. Run the server:
    ```bash
    go run main.go
    ```
4. The server starts on port 8080.

## Endpoints

- `GET /movies`: Get all movies.
- `GET /movies/{id}`: Get a single movie by ID.
- `POST /movies`: Create a new movie.
- `PUT /movies/{id}`: Update a movie by ID.
- `DELETE /movies/{id}`: Delete a movie by ID.

## Example Movie JSON

Here is an example of a movie in JSON format:

```json
{
    "id": "3",
    "isbn": "987654",
    "title": "The Dark Knight",
    "director": {
        "firstname": "Christopher",
        "lastname": "Nolan"
    }
}
```

Another example with a different director:

```json
{
    "id": "4",
    "isbn": "123789",
    "title": "Schindler's List",
    "director": {
        "firstname": "Steven",
        "lastname": "Spielberg"
    }
}
```

## Project Structure
- `main.go`: Contains all the code for the CRUD operations and server setup.

## Purpose
This project was created to get a solid foundation on Go structs, slices, and slice manipulation, without the complexity of integrating a database. It serves as a learning tool for Go's data structures and basic web server capabilities.