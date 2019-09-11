# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint           | What does this do? |
|--------|--------------------|--------------------|
| `GET`  | `/users`           | `This returns 5 users listing both their ID# and their User Name. It also informs the requester that there were no errors in their request.`|
| `GET`  | `/users/<user-id>` | `It returns an alert letting the requester know that there are no instaces of what they were looking for at that endpoint because there are no parameters with the title "user-id". It also returns a notification for the requester to let them know there were no errors made in their request attempt... HOWEVER, replacing <user-id> with the "username" of an existing member will display that specific user if they exist in the server. Using just their user "id" number does not work.`|
| `POST`  | `/users/signup`   | `Posting to this endpoint without parameters declaring the user name and id # of a new user brings an error message explaining that the requester needs to include these parameters to be able to post in this fashion.`|


* Fill in the blanks above :arrow_up: 

#### Todos
| Method   | Endpoint           | What does this do? | Possible Query Params |
|----------|--------------------|--------------------|-----------------------|
| `GET`    | `/todos`           | `This returns a list of six todo items by three authors, including their ID, the user name of the owner under "owner", the text of their todo item, and a qualifier letting the requester see if the todo item has been completed or not.`| `username=<username>`, `completed=<true|false> `
| `POST`   | `/todos`           | `This allows requesters to post items to the todo list. However, you need to specify the parameters "owner" (existing users only) and "text" (the note attached with the reminder for the user's todo list library)`||
| `GET`    | `/todos/<todo-id>` | `This allows the requester (with the specific server generated todo-id to read the entierety of the information housed in the todo item at that specific id`||
| `PUT`    | `/todos/<todo-id>` | `This allows the requester to change the entirety of thie todo item housed at the specific todo-id. This change is permanant, and if it is missing any information - it will omit that information in the update.`||
| `PATCH`  | `/todos/<todo-id>` | `This allows a requester to change the data housed in only one parameter without altering or removing any of the other data housed at that todo-id.`||
| `DELETE` | `/todos/<todo-id>` | `This removes the todo item at this todo-id completely. It can not be recovered.`||

* Fill in the blanks above :arrow_up: 

## Tasks
1. Try out all the requests that are possible with this API. For all the possible requests Create a list like the following.
Separate requests by a long line of underscores.
    * **Request**: METHOD - ENDPOINT
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      {
        "owner": "alejo4373",
        "text": "1st Todo"
      }
    ```
    * **Response**:
    ```json
    {
      "userId": 1,
      "id": 1,
      "title": "delectus aut autem",
      "completed": false
    }
    ```
    * **What does it do?**: EXPLAIN WHAT THE REQUEST DID/DO IN PLAIN ENGLISH

2. Find as much status codes as possible. I will tell you how many there are by the end.


DOUG'S ANSWER ZONE ============================================================

GET - /users

BODY
(no body)

RESPONSE
```json
{
    "payload": [
        {
            "id": 1,
            "username": "alejo4373"
        },
        {
            "id": 2,
            "username": "JRJRocks"
        },
        {
            "id": 3,
            "username": "Mike923"
        }, ...
}
```

WHAT DOES IT DO?
This requests all of the users currently created in the server by id# (system generated) and the "username"

-----------------------------------------------------------------------------

POST - /users

BODY
(does not matter)

RESPONSE
```json
{
    "payload": "Nah, nah, nah",
    "err": true
}
```

WHAT DOES IT DO?
Sends a request to create a data point at the "users" endpoint, but those accessing the API are blocked from creating anything directly at this endpoint.

-----------------------------------------------------------------------------

PUT - /users

BODY
(does not matter)

RESPONSE
```json
{
    "payload": "Nah, nah, nah",
    "err": true
}
```

WHAT DOES IT DO?
Requests a complete change/update to a specific user - however this method is blocked by the API, even if calling a specific user by ther username in the body.

-----------------------------------------------------------------------------

PATCH - /users

BODY
(does not matter)

RESPONSE
```json
{
    "payload": "Nah, nah, nah",
    "err": true
}
```

WHAT DOES IT DO?
Requests a partial change/update to a specific user - however, this method is blocked by the API.

-----------------------------------------------------------------------------

DELETE - /users

BODY
(no body)

RESPONSE
```json
{
    "payload": "Nah, nah, nah",
    "err": true
}
```

WHAT DOES IT DO?
Requests a datapoint be removed from the server, but this method is blocked by the API - even if a specific user is named in the body

-----------------------------------------------------------------------------

GET - users/signup

BODY
(no body)

RESPONSE
```json
{
    "payload": "What you where looking for was not found.",
    "err": false
}
```

WHAT DOES IT DO?
Requests to read/display data from this endpoint, but there is no information to display, so it sends a message to the requester letting them know nothing's there.

-----------------------------------------------------------------------------

POST - users/signup

BODY
```json
{
    "username": "GrilledCheeseFan93"
}
```

RESPONSE
```json
{
    "payload": {
        "user": {
            "id": 61,
            "username": "GrilledCheeseFan93"
        },
        "msg": "User created"
    },
    "err": false
}
```

WHAT DOES IT DO?
Requests a new datapoint be created at the /signup endpoint. It takes in the body parameter of "username":"<username>" and creates a new user instance. It applies the unique user name entered and autogenerates an id#. It also gives the requester two messages - one to let them know specifically that a new user was created, and the other to let them know that there were no errors.

-----------------------------------------------------------------------------

PUT - /users/signup

BODY
```json
(doesn't matter)
```

RESPONSE
```json
{
    "payload": "What you where looking for was not found.",
    "err": false
}
```

WHAT DOES IT DO?
Requests a complete removal/replacement of a datapoint with updated information. This method is blocked from this endpoint

-----------------------------------------------------------------------------

PATCH - users/signup

BODY
```json
(doesn't matter)
```

RESPONSE
```json
{
    "payload": "What you where looking for was not found.",
    "err": false
}
```

WHAT DOES IT DO?
Requests that a partial change of a datapoint be made - changing some of the data without altering/removing keys or values. This method is blocked at this endpoint.

-----------------------------------------------------------------------------

DELETE - users/signup

BODY
```json
(doesn't matter)
```

RESPONSE
```json
{
    "payload": "What you where looking for was not found.",
    "err": false
}
```

WHAT DOES IT DO?
Requests a datapoint be removed from this endpoint of the server. This method is blocked at this endpoint

-----------------------------------------------------------------------------

GET - /todos

BODY
```json
(no body)
```

RESPONSE
```json
{
    "payload": [
        {
            "id": "a3d4d7d0",
            "owner": "NewNew",
            "text": "Feed me Seymour! No seriously put dishes in me...",
            "completed": false
        },
        {
            "id": "ecf57050",
            "owner": "AnimalCrackerEater",
            "text": "Leave Crackers on the sofa",
            "completed": false
        },
        {
            "id": "07a5eaa0",
            "owner": "Stink Meaner",
            "text": "why delete",
            "completed": false
        }, ...
}
```

WHAT DOES IT DO?
Requests to read/display all the datapoints from this endpoint. (Lists all todos in the server.)

-----------------------------------------------------------------------------

POST - /todos

BODY
```json
{
    "owner": "Roscoe Merryweather",
    "text": "Crack safe",
    "completed": "true"
}
```

RESPONSE
```json
{
    "payload": {
        "id": "8a3d6540",
        "owner": "Roscoe Merryweather",
        "text": "crack safe",
        "completed": false
    },
    "err": false
}
```

WHAT DOES IT DO?
Requests a new datapoint be created at this endpoint. With the correct parameters (owner=registered-user, text=todo-item, completed=true/false), a new todo item will be added for the called user.

-----------------------------------------------------------------------------

PUT - /todos

BODY
```json
(Does not matter)
```

RESPONSE
```json
{
    "payload": "Nah, nah, nah",
    "err": true
}
```

WHAT DOES IT DO?
Attempts to overwrite a datapoint at the endpoint todos. The request is blocked, and a status message is displayed.

-----------------------------------------------------------------------------

PATCH - /todos

BODY
```json
(does not matter)

```

RESPONSE
```json
{
    "payload": "Nah, nah, nah",
    "err": true
}
```

WHAT DOES IT DO?
Attempts to partially update data within this datapoint housed at this endpoint. this request is blocked, and a status message is displayed.

-----------------------------------------------------------------------------

DELETE - /todos

BODY
```json
(does not matter)
```

RESPONSE
```json
{
    "payload": "Nah, nah, nah",
    "err": true
}
```

WHAT DOES IT DO?
Attempts to delete a datapoint from this endpoint. This request is blocked, and status message is displayed.

-----------------------------------------------------------------------------

GET - /todos/8a3d6540

BODY
```json
(no body)
```

RESPONSE
```json
{
    "payload": {
        "id": "8a3d6540",
        "owner": "Roscoe Merryweather",
        "text": "crack safe",
        "completed": false
    },
    "err": false
}
```

WHAT DOES IT DO?
Requests the datapoint at this endpoint be displayed. This requires the unique ID generated by the post of a new todo item.

-----------------------------------------------------------------------------

POST - /todos/8a3d6540

BODY
```json
(doesn't matter)
```

RESPONSE
```json
{
    "payload": "What you were looking for was not found. The endpoint or method is unhandled by the Server",
    "err": true
}
```

WHAT DOES IT DO?
Attempts to create a new datapoint at this endpoint, but since this is a datapoint inhabited by a uniue system assigned id, this request is blocked and a status message is displayed.

-----------------------------------------------------------------------------

PUT - /todos/8a3d6540

BODY
```json
{
    "owner": "Roscoe Merryweather",
    "text": "Eat a donut",
    "completed": "true"
}
```

RESPONSE
```json
{
    "payload": {
        "id": "8a3d6540",
        "owner": "Roscoe Merryweather",
        "text": "Eat a donut",
        "completed": true
    },
    "err": false
}
```

WHAT DOES IT DO?
Requests to fully change an endpoint, and requires all of the parameters before it will allow this method to be used (owner, text, and completed). It displays the updated datapoint if the requsites are complete.

-----------------------------------------------------------------------------

PATCH - /todos/8a3d6540

BODY
```json
{
    "text": "Bust out of jail"
}
```

RESPONSE
```json
{
    "payload": {
        "id": "8a3d6540",
        "owner": "Roscoe Merryweather",
        "text": "Bust out of jail",
        "completed": true
    },
    "err": false
}
```

WHAT DOES IT DO?
Requests a partial change of a datapoint (only text, as shown in the body). The update is commited and displayed

-----------------------------------------------------------------------------

DELETE - /todos/4dd2b090

BODY
```json
(no body)
```

RESPONSE
```json
{
    "payload": {
        "id": "4dd2b090",
        "owner": "Roscoe Merryweather",
        "text": "Rescue comet the wonder horse.",
        "completed": false
    },
    "err": false
}
```

WHAT DOES IT DO?
Removes a datapoint at this endpoint, and displays the removed datapoint.

-----------------------------------------------------------------------------

GET - /todos/4dd2b090

BODY
```json
(no body)
```

RESPONSE
```json
{
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}
```

WHAT DOES IT DO?
Since the datapoint was removed by the Delete Method, there is nothing found. A status message explaining such is displayed.

-----------------------------------------------------------------------------


### Bonuses
1. Take a look at the next lesson. To learn how to make make network requests with Javascript
Since you previously had build a simple Todos APP with HTML try to connect that app to this
API so that todos you enter in the page are save to the API. Marking a todo as complete or uncompleted
should work.
2. Find the easter egg.