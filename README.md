# Bookshelf API Projects
This is my first project on API which is Bookshelf API. This API is built using NodeJS and uses a framework, namely the Hapi Framework. There are 5 main criteria, namely the first API can store books, the second is the API can display all books, then the third is the API can display book details, after that the fourth is the API can change book data, and the last is the fifth API can delete books.

## Server<br>
The first is the server, on the server itself created via the Hapi.server() method. This method accepts one parameter, namely ServerOptions. ServerOptions is an object that holds the configuration of the server to be created, one of which can set port and host properties. The process of running the server is done asynchronously. Therefore it is necessary to run in an async function and call server.start() using await. After the server is running successfully, it can be seen through the full address and port of the server where the server is running through the server.info.uri properti property

## Routes<br>
In order for the web server to store books, it is necessary to provide a route with the path books and the 'POST' method. To be able to delete a book, a 'DELETE' method is needed. To be able to edit a book, you need the 'PUT' method. To be able to display the book, use the 'GET' method with the getAllBookHandler handler. Then to be able to make changes to the book using the 'GET' method with the path /books/{bookId} with the getBookByIdHandler handler.

## Handler <br>
Handler is a to handle requests. Each route specification has its own handler, so the code will be easier to manage.

## Books
Books.js is an array that serves to hold objects in books.