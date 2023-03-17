# go-crud-api-for-books
This is a simple CRUD API in Go using the Gorilla Mux router. It provides endpoints to create, read, update and delete books from a book list.

## Usage
To use this API, you can send HTTP requests to the following endpoints:
- GET `/books`: get a list of all books
- GET `/books/`{id}: get a specific book by its ID
- POST `/books`: create a new book
- PUT `/books/{id}`: update a book by its ID
- DELETE `/books/{id}`: delete a book by its ID

To **access the API**, send requests to the following URL: 
```
http://ec2-65-1-223-223.ap-south-1.compute.amazonaws.com:8080/books
```

You can use Postman tool to send HTTP requests to the API. Here are some examples of HTTP requests you can send:
### 1. GET `/books`
To get a list of all books, send a GET request to below address: 
```
http://ec2-65-1-223-223.ap-south-1.compute.amazonaws.com:8080/books
```
![image](https://user-images.githubusercontent.com/106534693/225952791-e6c9cba7-2e35-4189-8777-4d7980650268.png)

### 2. POST `/books`
To create a new book, send a POST request to  
```
http://ec2-65-1-223-223.ap-south-1.compute.amazonaws.com:8080/books
```
with the following JSON payload:
```
{
  "id": "2",
  "title": "Meghdutam",
  "author": "Kalidas"
}
```
![image](https://user-images.githubusercontent.com/106534693/225953152-1001fd9f-ac4d-4cf1-9f78-d00295e400b8.png)

### 3. GET `/books/{id}`
To get a specific book by its ID, replace {id} with the ID of the book you want to retrieve, and send a GET request to the following address:
```
http://ec2-65-1-223-223.ap-south-1.compute.amazonaws.com:8080/books/{id}
```
![image](https://user-images.githubusercontent.com/106534693/225953299-06a455cf-50bb-4e65-a166-ab67eec1487a.png)

### 4. PUT `/books/{id}`
To update a book by its ID, replace {id} with the ID of the book you want to update, and send a PUT request to 
```
http://ec2-65-1-223-223.ap-south-1.compute.amazonaws.com:8080/books/{id}
```
with the following JSON payload:
```
{
  "id": "2",
  "title": "Abhigyan Shakunltalam",
  "author": "Kalidas"
}
```
![image](https://user-images.githubusercontent.com/106534693/225953778-f3f90d8e-4f50-4ebc-8f59-94f67420dbc2.png)

### 5. DELETE `/books/{id}`
To delete a book by its ID, replace {id} with the ID of the book you want to delete, and send a DELETE request to 
```
http://ec2-65-1-223-223.ap-south-1.compute.amazonaws.com:8080/books/{id}
```
![image](https://user-images.githubusercontent.com/106534693/225954208-d18e90b9-b691-4e47-8803-d6313c6c96a5.png)

## Conclusion
In conclusion, this repository provides a simple CRUD API for managing a list of books, written in Go and deployed on an Amazon EC2 instance. Users can access the API by sending HTTP requests to the URL `http://ec2-65-1-223-223.ap-south-1.compute.amazonaws.com:8080/books` using a tool like Postman or Google Chrome. The API allows users to create, read, update, and delete books from the list.
