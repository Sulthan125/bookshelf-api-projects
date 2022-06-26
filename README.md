# Bookshelf API Projects
This is my first project on API which is Bookshelf API. This API is built using NodeJS and uses a framework, namely the Hapi Framework. There are 5 main criteria, namely the first API can store books, the second is the API can display all books, then the third is the API can display book details, after that the fourth is the API can change book data, and the last is the fifth API can delete books.

## Server<br>
The first is the server, on the server itself created via the Hapi.server() method. This method accepts one parameter, namely ServerOptions. ServerOptions is an object that holds the configuration of the server to be created, one of which can set port and host properties. The process of running the server is done asynchronously. Therefore it is necessary to run in an async function and call server.start() using await. After the server is running successfully, it can be seen through the full address and port of the server where the server is running through the server.info.uri properti property

## 