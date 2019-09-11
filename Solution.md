# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint           | What does this do? |
|--------|--------------------|--------------------|
| `GET`  | `/users`           | `_________________`|
| `GET`  | `/users/<username>` | `_________________`|
| `POST`  | `/users/signup`   | `_________________`|


* Fill in the blanks above :arrow_up: 

#### Todos
| Method   | Endpoint           | What does this do? | Possible Query Params |
|----------|--------------------|--------------------|-----------------------|
| `GET`    | `/todos`           | `_________________`| `owner=<username>`, `completed=<true|false> `
| `POST`   | `/todos`           | `_________________`||
| `GET`    | `/todos/<todo-id>` | `_________________`||
| `PUT`    | `/todos/<todo-id>` | `_________________`||
| `PATCH`  | `/todos/<todo-id>` | `_________________`||
| `DELETE` | `/todos/<todo-id>` | `_________________`||

* Fill in the blanks above :arrow_up: 

## Tasks
1. Try out all the requests that are possible with this API. For all the possible requests Create a list like the following.
Separate requests by a long line of underscores.
    * **Request**: POST - /users/signup	
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      username:A
    ```
    * **Response**:
    ```json
    {
    "payload": {
        "user": {
            "id": 19,
            "username": "A"
        },
        "msg": "User created"
    },
    "err": false
    }
    ```
    * **What does it do?**: Creates a new user.
=============================================================================== 
    * **Request**: GET - /users
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
        },
        {
            "id": 13,
            "username": " chrissyteigen"
        },
        {
            "id": 14,
            "username": "\"not alejo4373\""
        },
        {
            "id": 15,
            "username": "jenesh"
        },
        {
            "id": 16,
            "username": "22 Savage"
        },
        {
            "id": 17,
            "username": " Peter"
        },
        {
            "id": 18,
            "username": " test"
        },
        {
            "id": 19,
            "username": "A"
        },
        {
            "id": 20,
            "username": "Lil Thanos"
        },
        {
            "id": 21,
            "username": "Cow"
        },
        {
            "id": 22,
            "username": "Karen123"
        },
        {
            "id": 23,
            "username": "test2"
        },
        {
            "id": 24,
            "username": "Run The Jewels"
        }
      ],
      "err": false
    }
    ```
    * **What does it do?**: Gives the list of all users (with their ids).
=============================================================================== 
    * **Request**: GET - /users/A
    * **Body** (if applicable POST/PUT/PATCH)
    * **Response**:
    ```json
      {
        "payload": {
          "id": 19,
          "username": "A"
        },
        "err": false
      }
    ```
    * **What does it do?**: Gives the specified user with his/her id.
=============================================================================== 
    * **Request**: GET - /todos
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
    {
      completed:true
    }
    ```
    * **Response**:
    ```json
    {
      "payload": [
        {
            "id": "666",
            "owner": "Cow",
            "text": "Feed me Seymour! No seriously put dishes in me...",
            "completed": true
        },
        {
            "id": "1234567890",
            "owner": " Aransa",
            "text": "hola como estas? ",
            "completed": true
        },
        {
            "id": "fd3a5dd0",
            "owner": "the real not alejo4373",
            "text": "stare blankly at Postman for HOURS",
            "completed": true
        },
        {
            "id": "7",
            "owner": "okurrrt",
            "text": " ummm idk what to do",
            "completed": true
        },
        {
            "id": "31786e60",
            "owner": "Mike923",
            "text": "found who did it !!!!!!!!!",
            "completed": true
        },
        {
            "id": "5b26e2d0",
            "owner": "baconeggandcheese",
            "text": "two words",
            "completed": true
        }
      ],
      "err": false
    }
    
    ```
    * **What does it do?**: Gives a list of all the todos stored in the server.
=============================================================================== 
    * **Request**: POST - /todos
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      //id:19
      owner:A
      completed:false
      text:Get this lab done
    ```
    * **Response**:
    ```json
    {
      "payload": {
        "id": "40e882e0",
        "owner": "A",
        "text": "Get this lab done",
        "completed": false
      },
      "err": false
    }
    ```
    * **What does it do?**: Created a new todo under the user A
=============================================================================== 
    * **Request**: GET - /todos/40e882e0
    * **Body** (if applicable POST/PUT/PATCH)
    * **Response**:
    ```json
    {
      "payload": {
        "id": "40e882e0",
        "owner": "A",
        "text": "Get this lab done",
        "completed": false
      },
      "err": false
    }
    ```
    * **What does it do?**: Gives the todo what the id was specified on the request
=============================================================================== 
    * **Request**: PUT - /todos/40e882e0
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      //id:19
      owner:A
      completed:false
      text:Get this lab done↵Half way done
    ```
    * **Response**:
    ```json
    {
      "payload": {
        "id": "40e882e0",
        "owner": "A",
        "text": "Get this lab done\nHalf way done",
        "completed": false
      },
      "err": false
    }
    ```
    * **What does it do?**: Updates the todo which the id was on the request (
      all key/values must be inclued on the request)
=============================================================================== 
    * **Request**: PATCH - /todos/40e882e0
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      //id:19
      text:Get this lab done↵Getting there slowly
    ```
    * **Response**:
    ```json
    {
      "payload": {
        "id": "40e882e0",
        "owner": "A",
        "text": "Get this lab done\nGetting there slowly ",
        "completed": false
      },
      "err": false
    }
    ```
    * **What does it do?**: Updates the todo which the id was on the request with the key/value provided
=============================================================================== 
    * **Request**: DELETE - /todos/40e882e0
    * **Body** (if applicable POST/PUT/PATCH)
    * **Response**:
    ```json
    {
      "payload": {
        "id": "40e882e0",
        "owner": "A",
        "text": "Get this lab done\nGetting there slowly ",
        "completed": false
      },
      "err": false
    }
    ```
    * **What does it do?**: Delete the todo which the id was on the request.
===============================================================================   
2. Find as much status codes as possible. I will tell you how many there are by the end.
  * **201 created**: when creating a new user/todo
  * **200 OK**: for all other working requests
  * **404 not found**: for bad endopoints
  * **400 Bad request**: when trying to add a new todo but put key: username instead of owner or not all values are included
  * **409 conflict**: when trying to create a new user with a username already existing.
  * **500 Internal Server Error**: when trying to patch the id of my todo or when creating a new todo with an id that already exists.


### Bonuses
1. Take a look at the next lesson. To learn how to make make network requests with Javascript
Since you previously had build a simple Todos APP with HTML try to connect that app to this
API so that todos you enter in the page are save to the API. Marking a todo as complete or uncompleted
should work.
2. Find the easter egg.
