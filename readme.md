Sample application to demonstrate the power of api using go lang.

build the applicaiton by running

    gradle build

Run the application in localhost: 

    .\gorestapi.exe

The api exposes some endpoints to play with book manager. It accesses, add, delete books present in the repository.

`Use Postman to test below endpoints.`

http://localhost:8001/api/books

Endpoints:
1) GET - list the books

    `http://localhost:8001/api/books`

2) GET book by ID 

    ```http://localhost:8001/api/books/3```

3) POST - Create a book entry

    ```http://localhost:8001/api/books```
        
        sample payload - 
        {
            "isbn":"4565458",
            "title": "Book Four",
            "author": {
                "firstname": "Jairo",
                "lastname": "Quintana"
            }
        }

4) DELETE - remove a book  by ID

    `http://localhost:8001/api/books/2`
    
    here 2 is the book id which will be deleted


5) PUT- Update a book

    `http://localhost:8001/api/books`

        sample payload - 
        {
            "id": "2",
            "isbn": "256860000",
            "title": "Book Two00000",
            "author": {
                "firstname": "Ambuj000",
                "lastname": "Mondal0000"
            }
        }