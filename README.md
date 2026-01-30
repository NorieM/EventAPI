### Event Booking REST API with Golang

Using Gin framework, sqlite3

##### Endpoints

| Request Type | Endpoint | Description| Security |
| ------------ | -------- | ---------- | -------- |
| GET | /events                     | get a list of available events  |
| GET | /events/<id>                | get an event by id              |
| POST | /events                    | create an event  | Auth Required
| PUT | /events/<id>                | update an event  | Auth Required
| DELETE | /events/<id>             | delete an event  | Auth Required
| POST | /signup                    | create new user  | 
| POST | /login                     | authenicate user  | Auth Token (JWT)
| POST | /events/<id>/register      | register user for event  | Auth Required
| DELETE | /events/<id>/register    | cancel registration  | Auth Required


##### Installing Gin

Run this in the Terminal to install Gin:

go get -u github.com/gin-gonic/gin

#### Event Model

Fields
| Name        | Type      |
| ----------- | --------- |
| ID          | int       |
| Name        | string    |
| Description | string    |
| Location    | string    |
| DateTime    | time.Time |
| UserID      | int       |

Methods

Save - saves an event

#### Database

Uses sqlite

go get github.com/mattn/go-sqlite3


#### Security

go get -u golang.org/x/crypto