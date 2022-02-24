# REST-API using Golang(gorilla/mux package) with PostgreSQL DB

REST-API establishes create, read and delete (CRUD) operations and HTTP methods.

This REST-API is made for saving Movie names with their Id's in the database.

- GET = Retrieve all events or data from the database
- POST = Create a event or add data to the database.
- DELETE = Delete all/any events/event from the database.

Change the database User, Password and the Name:
```
  DB_USER     = "_USER_"
  DB_PASSWORD = "_PASSWORD_"
  DB_NAME     = "_NAME_"
 ```

Commands/URLs:

 GET :
 ```
  curl -X /movies
 ```
   or
 ```
  curl -X GET /movies
 ```
  
 POST :
 
 ```
  curl -H "Content-Type: application/json" -X POST /movies -d '{"movieid":"_ID_","moviename":"_MOVIENAME_"}'
 ```
 
 DELETE:
 - Delete a single movie record
 ```
  curl -X DELETE /movies/{movieid}
 ```
 - Delete all movie records
 ```
  curl -X DELETE /movies
 ```
  
