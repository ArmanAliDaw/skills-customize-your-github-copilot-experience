# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a small REST API with FastAPI that manages books in memory. Practice defining API routes, validating request data with Pydantic, and using HTTP methods and status codes.

## 📝 Tasks

### 🛠️ Create the books API

#### Description
Create a FastAPI application that lets clients list books and add new books. Each book should have an integer ID, a title, and an author.

#### Requirements
Completed program should:

- Install FastAPI and Uvicorn, and create the application in `main.py`.
- Define a Pydantic model that requires a non-empty title and author for new books.
- Implement `GET /books` to return all books and `POST /books` to add a book.
- Assign each new book a unique integer ID and return HTTP `201 Created` when it is added.
- Start the app with `uvicorn main:app --reload` and make the interactive API docs available at `/docs`.

### 🛠️ Add book detail and editing routes

#### Description
Extend the API so clients can retrieve, replace, and remove an individual book by its ID.

#### Requirements
Completed program should:

- Implement `GET /books/{book_id}` to return the matching book.
- Implement `PUT /books/{book_id}` to replace a book's title and author.
- Implement `DELETE /books/{book_id}` to remove a book.
- Return HTTP `404 Not Found` when a requested book ID does not exist.
- Return an appropriate success status for each route, including `204 No Content` after a successful delete.

### 🛠️ Test the API

#### Description
Exercise the API using its interactive documentation and write automated tests for its main behaviors.

#### Requirements
Completed program should:

- Use `/docs` to create, list, retrieve, update, and delete a book.
- Write tests with FastAPI's `TestClient` for creating a book and retrieving it.
- Test that requests for a missing book return HTTP `404 Not Found`.
- Confirm that invalid book data is rejected with a client error response.