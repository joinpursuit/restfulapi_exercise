# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint           | What does this do? |
|--------|--------------------|--------------------|
| `GET`  | `/users`           | `This returns a list of all available users in the api`|
| `GET`  | `/users/<user-id>` | `This returns information about a specific user based on user id`|
| `POST`  | `/users/signup`   | `This creates a new user`|


* Fill in the blanks above :arrow_up: 

#### Todos
| Method   | Endpoint           | What does this do? | Possible Query Params |
|----------|--------------------|--------------------|-----------------------|
| `GET`    | `/todos`           | `This returns toDos based on parameters defined`| `username=<username>`, `completed=<true|false> `
| `POST`   | `/todos`           | `Creates a new toDo`|| `id=<user-id>`, `toDos=<toDos>`
| `GET`    | `/todos/<todo-id>` | `Returns a todo based on the todo id provided`|| `todo-id=<todo-id>`, username=`<username>`
| `PUT`    | `/todos/<todo-id>` | `Replaces a todo based on the todo id provided`||  `todo-id=<todo-id>`, `username=<username>`
| `PATCH`  | `/todos/<todo-id>` | `Updates a todo based on the todo id provided`||  `todo-id=<todo-id>`, username=`<username>`
| `DELETE` | `/todos/<todo-id>` | `Deletes a todo based on the todo id provided`||  `todo-id=<todo-id>`, username=`<username>`

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

     * **Request**: GET -- /
    * **Body** N/A
    * **Response**:
    ```json
{
    "payload": "What you where looking for was not found.",
    "err": false
}
    ```
    * **What does it do?**: When a request to a endpoint that does not exist is made, this catchall endpoint catches it and returns this message to the user. 

      * **Request**: GET - users
    * **Body** (if applicable POST/PUT/PATCH)
    * **Response**:
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
        },
        {
            "id": 4,
            "username": "3Chainz"
        },
        {
            "id": 5,
            "username": "George W. Swoosh"
        },
        {
            "id": 6,
            "username": "A pimp named slickback"
        },
        {
            "id": 7,
            "username": "okurrrt"
        },
        {
            "id": 9,
            "username": "AnimalCrackerEater"
        },
        {
            "id": 10,
            "username": " SillyRabbit"
        },
        {
            "id": 11,
            "username": "Stink Meaner"
        },
        {
            "id": 12,
            "username": " theRealObama"
        }
    ],
    "err": false
}
    ```
    * **What does it do?**: Returns a list of all users in the api

    * **Request**: POST - users
    * **Body** {"username": "chuck Okonkwo"}
    * **Response**:
    ```json
{
    "payload": "Nah, nah, nah",
    "err": true
}
    ```
    * **What does it do?**: When a client attempts to post a new user to the api, the api returns a error message basically stating that the post method is not allowed 


    * **Request**: GET - users/username
    * **Response**:
    ```json
{
    "payload": {
        "id": 1,
        "username": "alejo4373"
    },
    "err": false
}
    ```


    * **Request**: GET - todos
    * **Response**:
    ```json
{
    "payload": {
        "id": 1,
        "username": "alejo4373"
    },
    "err": false
}
    ```
 * **Request**: POST -todos
 * **Response**:
    ```json
      {
            "id": "8feb0260",
            "owner": "the real not alejo4373",
            "text": "find edible food. profit!!!",
            "completed": false
        }
         ```
* **Request**: GET -todos/todo-id
 * **Response**:
    ```json
    {
    "payload": {
        "id": "2f77d8e0",
        "owner": "the real not alejo4373",
        "text": "look over at neighbor's screen to see if they're anywhere better in the lab",
        "completed": false
    },
    "err": false
}
         ```
         * **Request**: PUT -todos/todo-id
 * **Response**:
    ```json
    {
    "payload": {
        "id": "2f77d8e0",
        "owner": "the real not alejo4373",
        "text": "look over at neighbor's screen to see if they're anywhere better in the lab",
        "completed": false
    },
    "err": false
}
         ```


    





2. Find as much status codes as possible. I will tell you how many there are by the end.
200, 201, 405, 400, 401

### Bonuses
1. Take a look at the next lesson. To learn how to make make network requests with Javascript
Since you previously had build a simple Todos APP with HTML try to connect that app to this
API so that todos you enter in the page are save to the API. Marking a todo as complete or uncompleted
should work.
2. Find the easter egg.
