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
```json
    https://fsw62-todos-api.herokuapp.com/api/users
```
    * **Body** 
    
     ```json
     No body
     ```

    * **Response**:
    

     ```json
        {
            "id": 1,
            "username": "alejo4373"
        },
        {
            "id": 2,
            "username": "JRJRocks"
        },
    ```
    * **What does it do?**: EXPLAIN WHAT THE REQUEST DID/DO IN PLAIN ENGLISH
  GET requests simply return information stored at a specific endpoint. 
  it gives us the id's and the usernames


    ------------------------------------------------------

    ```json
    Request:
    https://fsw62-todos-api.herokuapp.com/api/users/alejo4373/
      ```
      ***body***

      No body

    ***response**:
    ```json
    {
    "payload": {
        "id": 1,
        "username": "alejo4373"
    },
    "err": false
}
```

--------------------------------------
  https://fsw62-todos-api.herokuapp.com/api/users/signup/

*** body**
yes I use body
x-wwwform-urlencoded
***response***

{
    "payload": {
        "user": {
            "id": 52,
            "username": "Sihame"
        },
        "msg": "User created"
    },
    "err": false
}

--------------------------------
***Todos***


```json
https://fsw62-todos-api.herokuapp.com/api/todos
```
***body**
```json
No body needed
```
***Response***
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
 ```

 https://fsw62-todos-api.herokuapp.com/api/todos/

{
    "payload": {
        "id": "4b0c7900",
        "owner": "Sihame",
        "text": "lol",
        "completed": false
    },
    "err": false
}


 https://fsw62-todos-api.herokuapp.com/api/todos/4b0c7900

{
    "payload": {
        "id": "4b0c7900",
        "owner": "Sihame",
        "text": "lol",
        "completed": false
    },
    "err": false
}



 https://fsw62-todos-api.herokuapp.com/api/todos/4b0c7900


{
    "payload": {
        "id": "4b0c7900",
        "owner": "Sihame",
        "text": "lol",
        "completed": true
    },
    "err": false
}

 https://fsw62-todos-api.herokuapp.com/api/todos/4b0c7900

{
    "payload": {
        "id": "4b0c7900",
        "owner": "Sihame",
        "text": "lab",
        "completed": true
    },
    "err": false
}


 https://fsw62-todos-api.herokuapp.com/api/todos/4b0c7900

{
    "payload": {
        "id": "4b0c7900",
        "owner": "Sihame",
        "text": "lab",
        "completed": true
    },
    "err": false
}

2. Find as much status codes as possible. I will tell you how many there are by the end.

### Bonuses
1. Take a look at the next lesson. To learn how to make make network requests with Javascript
Since you previously had build a simple Todos APP with HTML try to connect that app to this
API so that todos you enter in the page are save to the API. Marking a todo as complete or uncompleted
should work.
2. Find the easter egg.
