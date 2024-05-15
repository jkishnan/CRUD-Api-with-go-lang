Description:

This Go code implements a simple CRUD (Create, Read, Update, Delete) API for managing movie records. It utilizes the Gorilla Mux router for handling HTTP requests. The API allows users to perform the following operations:

1. **Retrieve all movies**: Sends a GET request to `/movies` to retrieve a JSON array of all movie records.
2. **Retrieve a single movie**: Sends a GET request to `/movies/{id}` to retrieve details of a specific movie identified by its ID.
3. **Create a new movie**: Sends a POST request to `/movies` with JSON data containing the details of the new movie to be created. The API generates a unique ID for the movie and adds it to the collection.
4. **Update an existing movie**: Sends a PUT request to `/movies/{id}` with JSON data containing the updated details of the movie identified by its ID.
5. **Delete a movie**: Sends a DELETE request to `/movies/{id}` to remove the movie record identified by its ID.

The data model includes two structs: `Movie` and `Director`. Each movie has an ID, ISBN, title, and director (which is an instance of the `Director` struct).

To run the server, execute the main function, which initializes the Gorilla Mux router, defines the API endpoints, and starts the server on port 8000.

README.md:

```
# Go Movies CRUD API

This Go code implements a simple CRUD (Create, Read, Update, Delete) API for managing movie records. It utilizes the Gorilla Mux router for handling HTTP requests.

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   ```

2. Navigate to the project directory:
   ```
   cd go-movies-crud
   ```

3. Install dependencies:
   ```
   go mod tidy
   ```

## Usage

To run the server, execute the following command:
   ```
   go run main.go
   ```

The server will start listening on port 8000.

## API Endpoints

- Retrieve all movies:
  ```
[  GET /movies](http://localhost:8000/movies)
  ```

- Retrieve a single movie by ID:
  ```
  GET /movies/{id}
  ```

- Create a new movie:
  ```
  POST /movies
  ```

- Update an existing movie by ID:
  ```
  PUT /movies/{id}
  ```

- Delete a movie by ID:
  ```
  DELETE /movies/{id}
  ```

## Dependencies

- [Gorilla Mux](https://github.com/gorilla/mux): A powerful URL router and dispatcher for Go.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or create a pull request.

