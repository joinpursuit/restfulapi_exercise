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
| `GET`  | `/users/<user-id>` | `_________________`|
| `POST`  | `/users/signup`   | `_________________`|


* Fill in the blanks above :arrow_up:

#### Todos
| Method   | Endpoint           | What does this do? | Possible Query Params |
|----------|--------------------|--------------------|-----------------------|
| `GET`    | `/todos`           | `_________________`| `username=<username>`, `completed=<true|false> `
| `POST`   | `/todos`           | `_________________`||
| `GET`    | `/todos/<todo-id>` | `_________________`||
| `PUT`    | `/todos/<todo-id>` | `_________________`||
| `PATCH`  | `/todos/<todo-id>` | `_________________`||
| `DELETE` | `/todos/<todo-id>` | `_________________`||

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
    ________________________________________________________________________________

    * **Request**: GET - https://fsw62-todos-api.herokuapp.com/api/users/
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
          }],
             "err": false
        }

    ```
    * **What does it do?**: shows the usernames

    ________________________________________________________________________________

    * **Request**: GET - https://fsw62-todos-api.herokuapp.com/api/users/ potato

    * **Response**:
    ```json

    {
        "payload": {
            "id": 48,
            "username": " potato"
        },
        "err": false
    }

    ```
    * **What does it do?**: return a specified user

    ________________________________________________________________________________

    * **Request**: POST - https://fsw62-todos-api.herokuapp.com/api/users/signup
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      {
        "username": "potato",

      }
    ```
    * **Response**:
    ```json

        {
        "payload": {
            "user": {
                "id": 48,
                "username": " potato"
            },
            "msg": "User created"
        },
        "err": false
    }

    ```
    * **What does it do?**: it added my username to the list

    ________________________________________________________________________________

    * **Request**: GET - https://fsw62-todos-api.herokuapp.com/api/todos

    * **Response**:
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
                "id": "33a3ebd0",
                "owner": "jenesh",
                "text": "spread radical candor",
                "completed": false
            }],

    "err": false}

    ```
    * **What does it do?**: returns all todo lists
    ________________________________________________________________________________

    * **Request**: POST - https://fsw62-todos-api.herokuapp.com/api/todos
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      {
        "owner": "potato",
        "text": "be a potato"

      }
    ```
    * **Response**:
    ```json

    {
        "payload": {
            "id": "0eebc0b0",
            "owner": " potato",
            "text": " be a potato",
            "completed": false
        },
        "err": false
    }

    ```
    * **What does it do?**: adds text to the specified username todo list
      ________________________________________________________________________________
      * **Request**: GET - https://fsw62-todos-api.herokuapp.com/api/todos/0eebc0b0

      * **Response**:
      ```json

      {
          "payload": {
              "id": "0eebc0b0",
              "owner": " potato",
              "text": " be a potato",
              "completed": false
          },
          "err": false
      }

      ```
      * **What does it do?**: returns the specified todo list using the id of the user

    ________________________________________________________________________________

    * **Request**: PUT - https://fsw62-todos-api.herokuapp.com/api/todos/0eebc0b0
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      {
        "text":"ya",
      "completed":"true",
      "id":"0eebc0b0",
      "owner": "potato"

      }
    ```
    * **Response**:
    ```json

    {
      "payload": {
          "id": "0eebc0b0",
          "owner": " potato",
          "text": "ya",
          "completed": true
      },
      "err": false
  }

    ```
    * **What does it do?**: changes the todo

    ________________________________________________________________________________

    * **Request**: PATCH - https://fsw62-todos-api.herokuapp.com/api/todos/0eebc0b0
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      {
    "text":"lallala"

      }
    ```
    * **Response**:
    ```json

    {
      "payload": {
          "id": "0eebc0b0",
          "owner": " potato",
          "text": "lallala",
          "completed": true
      },
      "err": false
  }

    ```
    * **What does it do?**: changes one part of the todo

    ________________________________________________________________________________

    * **Request**: DELETE - https://fsw62-todos-api.herokuapp.com/api/todos/0eebc0b0

    * **Response**:
    ```json

    {
      "payload": {
          "id": "0eebc0b0",
          "owner": " potato",
          "text": "lallala",
          "completed": true
      },
      "err": false
  }

    ```
    * **What does it do?**: deletes the todo


2. Find as much status codes as possible. I will tell you how many there are by the end.
200, 201, 404

### Bonuses
1. Take a look at the next lesson. To learn how to make make network requests with Javascript
Since you previously had build a simple Todos APP with HTML try to connect that app to this
API so that todos you enter in the page are save to the API. Marking a todo as complete or uncompleted
should work.
2. Find the easter egg.
