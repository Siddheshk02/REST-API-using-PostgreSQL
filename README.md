# REST-API using Golang(gorilla/mux package) with PostgreSQL DB

REST-API establishes create, read and delete (CRUD) operations and HTTP methods.

This REST-API is made for saving Movie names with their Id's in the database.

- GET = Retrieve all events or data from the database
- POST = Create a event or add data to the database.
- DELETE = Delete all/any events/event from the database.

Change the database 

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
 - delete a single movie record
 ```
  curl -X DELETE /movies/{movieid}
 ```
 - delete all movie records
 ```
  curl -X DELETE /movies
 ```
  
