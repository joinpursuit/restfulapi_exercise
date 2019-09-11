# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint           | What does this do? |
|--------|--------------------|--------------------|
| `GET`  | `/users`           | `this displays a user id and a username`
| `GET`  | `/users/<user-id>` | `A message pops up that states that what you were looking for is not found. If you remove the <>and input the user name, you get the information of the user`
| `POST`  | `/users/signup`   | `Creates a new user and adds it to the list on the payload list`


* Fill in the blanks above :arrow_up:

#### Todos
| Method   | Endpoint           | What does this do? | Possible Query Params |
|----------|--------------------|--------------------|-----------------------|
| `GET`    | `/todos`           | `Shows things on the todo list of different users.`
| `POST`   | `/todos`           | `This adds a username into the payload list.`
| `GET`    | `/todos/<todo-id>` | `Can specifically access a specific todo task`
| `PUT`    | `/todos/<todo-id>` | `Allows you to modify the whole todo item and appends it to the bottom of the list`
| `PATCH`  | `/todos/<todo-id>` | `Allows you to edit one point of your item.`
| `DELETE` | `/todos/<todo-id>` | `Deletes a post with the id number that was provided.`

* Fill in the blanks above :arrow_up:

## Tasks
1. Try out all the requests that are possible with this API. For all the possible requests Create a list like the following.
Separate requests by a long line of underscores.

**Request**: GET - /todos
**Body**: N/A
**Response**:
```json
"payload": [
     {
         "id": "ecf57050",
         "owner": "AnimalCrackerEater",
         "text": "Leave Crackers on the sofa",
         "completed": false
     },
     {
         "id": "33a3ebd0",
         "owner": "jenesh",
         "text": "spread radical candor",
         "completed": false
     },
     {
         "id": "5354dde0",
         "owner": "George W. Swoosh",
         "text": "Invade Iraq",
         "completed": false
     }]
```
**What does it do?**: Shows things on the todo list of different users.
_______________________________________________________________________________

  **Request**: POST - /todos
  **Body**:
  ```json
  {
    "id":7,
    "owner": "okurrrt",
    "text":"idk what to do anymore"
  }
  ```

  **Response**:
  ```json
  "payload": [
       {
           "id": "ecf57050",
           "owner": "AnimalCrackerEater",
           "text": "Leave Crackers on the sofa",
           "completed": false
       },
       {
           "id": "33a3ebd0",
           "owner": "jenesh",
           "text": "spread radical candor",
           "completed": false
       },
       {
           "id": "5354dde0",
           "owner": "George W. Swoosh",
           "text": "Invade Iraq",
           "completed": false
       },
       {
         "id":7,
         "owner": "okurrrt",
         "text":"idk what to do anymore"
       }]
  ```
  **What does it do?**: This adds a username into the payload list.
_______________________________________________________________________________

**Request**: GET - /todos/<todos-id>
**Body**: N/A
**Response**:
```json
{
  "id":7,
  "owner": "okurrrt",
  "text":"idk what to do anymore"
}
```
**What does it do?**: Can specifically access a specific todo task
_______________________________________________________________________________

**Request**: PUT - todos/<todos-id>
**Body**:
```json
{
  "id": 7,
  "owner":"okurrrt",
  "text":"blahblahblah",
  "completed":"true"
}
```
**Response**:
```json
"payload": [
     {
         "id": "ecf57050",
         "owner": "AnimalCrackerEater",
         "text": "Leave Crackers on the sofa",
         "completed": false
     },
     {
         "id": "33a3ebd0",
         "owner": "jenesh",
         "text": "spread radical candor",
         "completed": false
     },
     {
         "id": "5354dde0",
         "owner": "George W. Swoosh",
         "text": "Invade Iraq",
         "completed": false
     },
     {
       "id":7,
       "owner": "okurrrt",
       "text":"idk what to do anymore",
       "completed":"true"
     }]
```
**What does it do?**: Allows you to modify the whole todo item and appends it to the bottom of the list
__________________________________________________________________________________

**Request**: PATCH - todos/<todos-id>
**Body**:
```json
{
  "text": "i'm confused",
}
```
**Response**:
```json
"payload": [
     {
         "id": "ecf57050",
         "owner": "AnimalCrackerEater",
         "text": "Leave Crackers on the sofa",
         "completed": false
     },
     {
         "id": "33a3ebd0",
         "owner": "jenesh",
         "text": "spread radical candor",
         "completed": false
     },
     {
         "id": "5354dde0",
         "owner": "George W. Swoosh",
         "text": "Invade Iraq",
         "completed": false
     },
     {
       "id":7,
       "owner": "okurrrt",
       "text":"i'm confused",
       "completed":"true"
     }]
```
**What does it do?**: Allows you to edit one point of your item.
________________________________________________________________________________

**Request***: DELETE - todos/<todos-id>
**Body**: N/A
**Response**:
```json
"payload": [
     {
         "id": "ecf57050",
         "owner": "AnimalCrackerEater",
         "text": "Leave Crackers on the sofa",
         "completed": false
     },
     {
         "id": "33a3ebd0",
         "owner": "jenesh",
         "text": "spread radical candor",
         "completed": false
     },
     {
         "id": "5354dde0",
         "owner": "George W. Swoosh",
         "text": "Invade Iraq",
         "completed": false
     }]
```
**What does it do?**: Deletes a post with the id number that was provided.

2. Find as much status codes as possible. I will tell you how many there are by the end.
"200" - "OK"
"201" - "created"
"403" - "forbidden"
"404" - "Not found"
"405" - "Nah, nah nah"

### Bonuses
1. Take a look at the next lesson. To learn how to make make network requests with Javascript
Since you previously had build a simple Todos APP with HTML try to connect that app to this
API so that todos you enter in the page are save to the API. Marking a todo as complete or uncompleted
should work.
2. Find the easter egg.
