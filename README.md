# bookstore

This application is a simple bookstore RESTful web service that allows users to retrieve and add books to the system. It is built using Java and the Spring Boot framework.

To use the application, you can start by cloning the repository from the command line:

```markup
git clone https://github.com/<username>/bookstore.git
```
Once you have the code, you can build and run the application using the following commands:

```markup
cd bookstore
./mvnw spring-boot:run
```
Once the application is up and running, you can interact with it using either cURL or Postman.

To add a book to the system using cURL, you can use the following command:

```markup
curl -X POST -H "Content-Type: application/json" -d '{"title": "The Great Gatsby", "author": "F. Scott Fitzgerald"}' http://localhost:8080/books
```
To add a book to the system using Postman, you can create a new POST request and set the request URL to http://localhost:8080/books. Then, you can set the request body to a JSON object with the book details, like so:

```json
{
"title": "The Great Gatsby",
"author": "F. Scott Fitzgerald"
}
```
Make sure to deselect the "Content-Type" header in the "Headers" tab, and then manually add it back with the value "application/json" so that Postman knows the request body is in JSON format.

To retrieve all books in the system, you can send a GET request to http://localhost:8080/books. This will return a JSON object with an array of book objects.

That's it! With this simple bookstore RESTful web service, you can easily add and retrieve books from the system using either cURL or Postman.
