### Event Booking REST API with Golang

Using Gin framework, sqlite3

##### Endpoints

| Request Type | Endpoint | Description|
| ------------ | -------- | ---------- |
| GET | /events                     | get a list of available events  
| GET | /events/<id>                | get an event by id  
| POST | /events                    | create an event  
| PUT | /events/<id>                | update an event  
| DELETE | /events/<id>             | delete an event  
| POST | /signup                    | create new user  
| POST | /login                     | authenicate user  
| POST | /events/<id>/register      | register user for event  
| DELETE | /events/<id>/register    | cancel registration  


##### Installing Gin

Run this in the Terminal to install Gin:

go get -u github.com/gin-gonic/gin

