# 📘 Assignment: Build a Web Client for Your FastAPI Book API

## 🎯 Objective

Build a small browser-based book catalog that communicates with the FastAPI books API from the previous assignment. Practice making HTTP requests with JavaScript `fetch` and handling API responses in a web page.

## 📝 Tasks

### 🛠️ Allow browser requests to the API

#### Description
Update your FastAPI application so a web page served locally can request the books API from the browser.

#### Requirements
Completed program should:

- Configure FastAPI's `CORSMiddleware` to allow the frontend origin `http://localhost:5500`.
- Allow the `GET` and `POST` methods and the `Content-Type` request header.
- Keep the API available at `http://127.0.0.1:8000`.

### 🛠️ Build the book catalog page

#### Description
Create an `index.html` page with JavaScript that loads books from the API and lets a visitor add a book.

#### Requirements
Completed program should:

- Include a labeled form with fields for a book title and author.
- Use `fetch` with `GET /books` to load and display each book's title and author.
- Use `fetch` with `POST /books` to submit a new book as JSON with the correct `Content-Type` header.
- Refresh the displayed list after a book is added successfully.
- Render book details as text rather than interpreting them as HTML.

### 🛠️ Run and verify the client

#### Description
Run the API and web page locally, then test the full workflow from the browser.

#### Requirements
Completed program should:

- Start the API with `uvicorn main:app --reload` and serve the page with `python -m http.server 5500` from the directory containing `index.html`.
- Open `http://localhost:5500` and confirm that existing books appear.
- Add a book through the form and confirm it appears in the catalog.
- Show a clear message if the API cannot be reached or rejects the submitted book.