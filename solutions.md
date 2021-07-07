# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint           | What does this do? |
|--------|--------------------|--------------------|
| `GET`  | `/users`           | `returns users`|
https://fsw62-todos-api.herokuapp.com/api/users

{
    "payload": [
        {
            "id": 1,
            "username": "alejo4373"
        }
    ],
    "err": false
}


| `GET`  | `/users/<user-id>` | `returns user info that you asked for`|
https://fsw62-todos-api.herokuapp.com/api/users/1

{
    "payload": [
        {
            "id": 1,
            "username": "alejo4373"
        }
    ],
    "err": false
}



| `POST`  | `/users/signup`   | `creates a new user`|
https://fsw62-todos-api.herokuapp.com/api/users/signup

{
    "payload": {
        "user": {
            "id": 13,
            "username": " chrissyteigen"
        },
        "msg": "User created"
    },
    "err": false
}



* Fill in the blanks above :arrow_up:

#### Todos
| Method   | Endpoint           | What does this do? | Possible Query Params |
|----------|--------------------|--------------------|-----------------------|
| `GET`    | `/todos`           | `returns all the todos`| `username=<username>`, `completed=<true|false> `
https://fsw62-todos-api.herokuapp.com/api/todos

{
    "payload": [
        {
            "id": "8c141120",
            "owner": "Mike923",
            "text": "wash dishes",
            "completed": false
        },
        {
            "id": "97ea0130",
            "owner": "Mike923",
            "text": "wash car",
            "completed": false
        },
        {
            "id": "209cf820",
            "owner": " theRealObama",
            "text": "hide birth certificate",
            "completed": false
        },
        {
            "id": "24e8f9b0",
            "owner": " theRealObama",
            "text": "hide birth certificate",
            "completed": false
        },
        {
            "id": "2665fcc0",
            "owner": " theRealObama",
            "text": "hide birth certificate",
            "completed": false
        },
        {
            "id": "5593ede0",
            "owner": "AnimalCrackerEater",
            "text": "Unwash dishes",
            "completed": false
        }
    ],
    "err": false
}



| `POST`   | `/todos`           | `creates a new todo`||
https://fsw62-todos-api.herokuapp.com/api/todos/

{
    "payload": {
        "id": " 13",
        "owner": " chrissyteigen",
        "text": " walk dog",
        "completed": false
    },
    "err": false
}


| `GET`    | `/todos/<todo-id>` | `returns specific todo that you asked for`||
https://fsw62-todos-api.herokuapp.com/api/todos/7

{
    "payload": {
        "id": "7",
        "owner": "okurrrt",
        "text": " meal prep",
        "completed": false
    },
    "err": false
}


| `PUT`    | `/todos/<todo-id>` | `allows you to change all keys, cannot change just one`||
https://fsw62-todos-api.herokuapp.com/api/todos/13
{
    "payload": {
        "id": " 13",
        "owner": " chrissyteigen",
        "text": " drink coffee",
        "completed": true
    },
    "err": false
}


| `PATCH`  | `/todos/<todo-id>` | `allows you to change only one key`||
https://fsw62-todos-api.herokuapp.com/api/todos/13

{
    "payload": {
        "id": " 13",
        "owner": " chrissyteigen",
        "text": " drink coffee",
        "completed": false
    },
    "err": false
}


| `DELETE` | `/todos/<todo-id>` | `deletes entire todo that you specified`||
https://fsw62-todos-api.herokuapp.com/api/todos/13

{
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}

## Tasks
1. Try out all the requests that are possible with this API. For all the possible requests Create a list like the following.
Separate requests by a long line of underscores.

**Request**: GET - https://fsw62-todos-api.herokuapp.com/api/users
**Response**:
{
    "payload": [
        {
            "id": 1,
            "username": "alejo4373"
        }
    ],
    "err": false
}
**What does it do?**: Returns users

____________________________________________________________________________________________

**Request**: GET - https://fsw62-todos-api.herokuapp.com/api/users/1
**Response**:
{
    "payload": [
        {
            "id": 1,
            "username": "alejo4373"
        }
    ],
    "err": false
}

**What does it do?**: Returns specific user you asked for

____________________________________________________________________________________________


**Request**: POST - https://fsw62-todos-api.herokuapp.com/api/users/signup
**Body**:
"user": {
    "id": 13,
    "username": " chrissyteigen"
},
**Response**:
{
    "payload": {
        "user": {
            "id": 13,
            "username": " chrissyteigen"
        },
        "msg": "User created"
    },
    "err": false
}
**What does it do?**: Creates a new user

____________________________________________________________________________________________

**Request**: GET - https://fsw62-todos-api.herokuapp.com/api/todos
**Response**:
{
    "payload": [
        {
            "id": "8c141120",
            "owner": "Mike923",
            "text": "wash dishes",
            "completed": false
        },
        {
            "id": "97ea0130",
            "owner": "Mike923",
            "text": "wash car",
            "completed": false
        },
        {
            "id": "209cf820",
            "owner": " theRealObama",
            "text": "hide birth certificate",
            "completed": false
        },
        {
            "id": "24e8f9b0",
            "owner": " theRealObama",
            "text": "hide birth certificate",
            "completed": false
        },
        {
            "id": "2665fcc0",
            "owner": " theRealObama",
            "text": "hide birth certificate",
            "completed": false
        },
        {
            "id": "5593ede0",
            "owner": "AnimalCrackerEater",
            "text": "Unwash dishes",
            "completed": false
        }
    ],
    "err": false
}


**What does it do?**: Returns all the todos

____________________________________________________________________________________________

**Request**: POST - https://fsw62-todos-api.herokuapp.com/api/todos/
**Body**:
{
  "id": " 13",
  "owner": " chrissyteigen",
  "text": " walk dog",
  "completed": false  
}
**Response**:
{
    "payload": {
        "id": " 13",
        "owner": " chrissyteigen",
        "text": " walk dog",
        "completed": false
    },
    "err": false
}
**What does it do?**: Creates a new todo

____________________________________________________________________________________________

**Request**: GET - https://fsw62-todos-api.herokuapp.com/api/todos/7
**Response**:
{
    "payload": {
        "id": "7",
        "owner": "okurrrt",
        "text": " meal prep",
        "completed": false
    },
    "err": false
}
**What does it do?**: Returns specific todo you asked for

____________________________________________________________________________________________

**Request**: PUT - https://fsw62-todos-api.herokuapp.com/api/todos/13
**Body**:
{
    "id": " 13",
    "owner": " chrissyteigen",
    "text": " drink coffee",
    "completed": true
},
**Response**:
{
    "payload": {
        "id": " 13",
        "owner": " chrissyteigen",
        "text": " drink coffee",
        "completed": true
    },
    "err": false
}
**What does it do?**: Allows you to change all keys, cannot change just one

____________________________________________________________________________________________

**Request**: PATCH - https://fsw62-todos-api.herokuapp.com/api/todos/13
**Body**:
{
    "completed": false
},
**Response**:
{
    "payload": {
        "id": " 13",
        "owner": " chrissyteigen",
        "text": " drink coffee",
        "completed": false
    },
    "err": false
}
**What does it do?**: Allows you to change only one key


____________________________________________________________________________________________


**Request**: DELETE - https://fsw62-todos-api.herokuapp.com/api/todos/13
**Response**:
{
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}
**What does it do?**: Deletes entire todo that you specified

____________________________________________________________________________________________

2. Find as much status codes as possible. I will tell you how many there are by the end.
There are 600.
