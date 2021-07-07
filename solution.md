| Method | Endpoint | What does this do?  |
| ------ | -------- | ------------------- |
| `GET`  | `/users` | `_________________` |

grabs user by the username
{
"payload": [
{
"id": 1,
"username": "alejo4373"
}
],
"err": false
}

| `GET` | `/users/<user-id>` | `_________________`|
grabs users by id
{
"payload": {
"id": 7,
"username": "okurrrt"
},
"err": false
}

| `POST` | `/users/signup` | `_________________`|
adds user to Users
{
"payload": {
"user": {
"id": 10,
"username": " SillyRabbit"
},
"msg": "User created"
},
"err": false
}

#### Todos

| Method | Endpoint | What does this do?  | Possible Query Params                           |
| ------ | -------- | ------------------- | ----------------------------------------------- |
| `GET`  | `/todos` | `_________________` | `username=<username>`, `completed=<true|false>` |

Grabs all of the entries in the todo list
{
"payload": [
{
"id": "8c141120",
"owner": "Mike923",
"text": "wash dishes",
"completed": false
},
],
"err": false
}

| `POST` | `/todos` | `_________________`||
creating a task and adding it to a user
{
"payload": {
"id": "8",
"owner": " SillyRabbit",
"text": " clean up",
"completed": false
},
"err": false
}

| `GET` | `/todos/<todo-id>` | `_________________`||
grabs entry using ID
{
"payload": {
"id": "8",
"owner": " SillyRabbit",
"text": " clean up",
"completed": true
},
"err": false
}

| `PUT` | `/todos/<todo-id>` | `_________________`||
changes part of the entry. needs all key and values to change
{
"payload": {
"id": "8",
"owner": " SillyRabbit",
"text": " clean up",
"completed": false
},
"err": false
}

| `PATCH` | `/todos/<todo-id>` | `_________________`||
changes part of the entry. just needs the part of the entry thats being modified
{
"payload": {
"id": "8",
"owner": " SillyRabbit",
"text": " clean up",
"completed": true
},
"err": false
}
| `DELETE` | `/todos/<todo-id>` | `_________________`||
https://fsw62-todos-api.herokuapp.com/api/todos/8
{
"payload": {
"msg": "Todo not found"
},
"err": true
}

## Tasks

1.  Try out all the requests that are possible with this API. For all the possible requests Create a list like the following.
    Separate requests by a long line of underscores.
    _ **Request**: METHOD - ENDPOINT
    https://fsw62-todos-api.herokuapp.com/api/todos/sillyrabbit
    _ **Response**:
    {
    "payload": {
    "user": {
    "id": 10,
    "username": " SillyRabbit"
    },
    "msg": "User created"
    },
    "err": false \* **What does it do?**: EXPLAIN WHAT THE REQUEST DID/DO IN PLAIN ENGLISH

        GET - grabs all entity in from the endpoint

- **Request**: METHOD - ENDPOINT

https://fsw62-todos-api.herokuapp.com/api/todos

- **Response**:
  {
  "payload": {
  "id": "8",
  "owner": " SillyRabbit",
  "text": " clean up",
  "completed": true
  },
  "err": false
  }

- **What does it do?**: EXPLAIN WHAT THE REQUEST DID/DO IN PLAIN ENGLISH
  POST - adding a entry in the todo api.

- **Request**: METHOD - ENDPOINT
  https://fsw62-todos-api.herokuapp.com/api/todos/8
- **Response**:
  {
  "payload": {
  "id": "8",
  "owner": " SillyRabbit",
  "text": " clean up",
  "completed": false
  },
  "err": false
  }
- **What does it do?**: EXPLAIN WHAT THE REQUEST DID/DO IN PLAIN ENGLISH
  PUT - modifies an entire entry even if its just a line that needs to be changed.

- **Request**: METHOD - ENDPOINT
  https://fsw62-todos-api.herokuapp.com/api/todos/8
- **Response**:
  {
  "payload": {
  "id": "8",
  "owner": " SillyRabbit",
  "text": " clean up",
  "completed": true
  },
  "err": false
  }
- **What does it do?**: EXPLAIN WHAT THE REQUEST DID/DO IN PLAIN ENGLISH
  PATCH- modifies only the line in the entry that needs to be changed

- **Request**: METHOD - ENDPOINT
  https://fsw62-todos-api.herokuapp.com/api/todos/8
- **Response**:
  {
  "payload": {
  "msg": "Todo not found"
  },
  "err": true
  }
- **What does it do?**: EXPLAIN WHAT THE REQUEST DID/DO IN PLAIN ENGLISH
  DELETE- removes entry from API.

  2. Find as much status codes as possible. I will tell you how many there are by the end.
     404 - "Not Found"
     200- "OK"
     405 - "Method not allowed"
     201 - "Created"
     204 - "No Content"
     403 - "Forbidden"
     400- "Bad Request"
