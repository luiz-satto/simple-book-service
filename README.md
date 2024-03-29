
Simple Book SPA
---
* This application is a simple service to deal with books (CRUD).
* This doesn't implement an entire library but just the basic structure to maintain a catalogue of books:

![image](https://github.com/luiz-satto/SimpleBookService/blob/main/Assets/simple-book-service-home.PNG)

## Create new book Page

![image](https://github.com/luiz-satto/SimpleBookService/blob/main/Assets/simple-book-service-create-new-book.PNG)

## Edit book details Page

![image](https://github.com/luiz-satto/SimpleBookService/blob/main/Assets/simple-book-service-edit-a-book.PNG)

## View book details Page

![image](https://github.com/luiz-satto/SimpleBookService/blob/main/Assets/simple-book-service-view-book-details.PNG)

Simple Book Service
---
> This project is using user-secrets to store the connection string details and connect to mongoDB
> Before run it go to the nuget packge manager console and then type:
```
dotnet user-secrets init
```

> Then:
```
dotnet user-secrets set "CONNECTION_STRING" "mongodb+srv://lsatto:82HJZEvQ8ahAuQ2j@simplebookservice.cnlz9.mongodb.net/SimpleBookServiceDb?retryWrites=true&w=majority"
```

> To check if the conn str is set you can type:
```
dotnet user-secrets list
```

Simple Book Service WebApi
---
* This API implement ***GetBook** endpoint to return the entire book structure back to the client by id
> [GET] **/GetBook/{id}**

* This API implement **GetBooks** endpoint to return all books back to the client
> [GET] **/GetBooks**

* This API implement **Create** endpoint to create a new book and return the new book id back to the client
> [POST] **/Create**

* This API implement Update endpoint to update an existing book and return the updated book structure back to the client
> [PUT] **Update/{id}**

* This API implement DeleteBookAsync endpoint to delete an existing book
> [DELETE] **Delete/{id}**
