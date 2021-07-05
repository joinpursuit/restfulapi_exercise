# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

***1.Get===> users:**
---------------------
    ***Request: METHOD - ENDPOINT***
```json
    https://fsw62-todos-api.herokuapp.com/api/users
```
======================================
    ***Body***
    
     ```json
     No body used
     ```
======================================
    ***Response***
    
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
======================================
    ***What does it do?***

```json

  GET requests simply return information stored at a specific endpoint. 
  it gives us the id's and the usernames

```
======================================
***status codes***

```json
status: 200 ok
```
--------------------------------------
***2.Get ===> user-username:**
-----------------------

 ***Request: METHOD - ENDPOINT***

```json

    https://fsw62-todos-api.herokuapp.com/api/users/alejo4373/
```

======================================
      ***body***
```json
No body needed
```
======================================
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
======================================
    ***What does it do?***

```json

  GET requests simply return information stored at a specific endpoint. 
  it gives us the id ,usernames and err of the user alejo4373 as we requested.

```
======================================
***status codes***

```json
status: 200 ok
```
--------------------------------------
***3.Post====>users/signup:**
-----------------------------
***Request: METHOD - ENDPOINT***
```json
  https://fsw62-todos-api.herokuapp.com/api/users/signup/
```
======================================
*** body**

* yes I use body because is Post method
* x-wwwform-urlencoded
* username: Sihame
* text: Having Fun
======================================
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
--------------------------------------
***What does it do?***

```json
POST is used to send data to a server to create or update a resource.
in our case we send data to a server. we create a new username and a text and their value
```
======================================
***status codes***

```json
status: 201 created
```
***3.Post====>users/signup:**
--------------------------------------

***Todos***

***1.GET====>/todos:**
-----------------------------
***Request: METHOD - ENDPOINT***

```json
https://fsw62-todos-api.herokuapp.com/api/todos
```
======================================
    ***Body***
    
     ```json
     No body used
     ```
======================================
***Response***

```json
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
======================================
    ***What does it do?***

```json

  GET  returns all users information stored at a todos endpoint. 
  it gives us the id's, owners, texts, and completed values.

```
======================================
***status codes***

```json
status: 200 ok

```
--------------------------------------
***2.POST====>/todos:**
-----------------------------
***Request: METHOD - ENDPOINT***
```json
 https://fsw62-todos-api.herokuapp.com/api/todos/
```
======================================
*** body**

* yes I use body because is Post method
* x-wwwform-urlencoded
* id: 4b0c7900
* owner: Sihame
* text: Having Fun
* completed: false
======================================
***Response***

```json
{
    "payload": {
        "id": "4b0c7900",
        "owner": "Sihame",
        "text": "lol",
        "completed": false
    },
    "err": false
}
```
======================================
***What does it do?***

```json
POST is used to update data to a resource.
```
======================================
***status codes***

```json
status: 201 created
```
--------------------------------------
***3.GET====>/todos/<todo-id>:**
-----------------------------
***Request: METHOD - ENDPOINT***
```json
 https://fsw62-todos-api.herokuapp.com/api/todos/4b0c7900
```
======================================
***Response***

{
    "payload": {
        "id": "4b0c7900",
        "owner": "Sihame",
        "text": "lol",
        "completed": false
    },
    "err": false
}
======================================
***Body***

```json
  No body used
```
======================================
    ***What does it do?***

```json

  GET  user id at t the endpoint to get information stored at a todos endpoint. 
  it gives us the id's, owners, texts, and completed values for the specific id information that we requested.

```
======================================
***status codes***

```json
status: 200 ok

```
--------------------------------------
***4.PUT====>/todos/<todo-id>:**
-----------------------------
***Request: METHOD - ENDPOINT***
```json
 https://fsw62-todos-api.herokuapp.com/api/todos/4b0c7900
 ```
======================================
***Response***

{
    "payload": {
        "id": "4b0c7900",
        "owner": "Sihame",
        "text": "lol",
        "completed": true
    },
    "err": false
}
======================================
***Body***

```json
  yes with put we have to use body
  x-wwwform-urlencoded
* id: 4b0c7900
* owner: Sihame
* text: lol
* completed: it was false and i update it to true

```
======================================
    ***What does it do?***

```json

  Put  user id at the endpoint to update all information for a specific ID

```
======================================
***status codes***

```json
status: 200ok

```
======================================
***5.Patch====>/todos/<todo-id>:**
--------------------------------
***Request: METHOD - ENDPOINT***
```json
 https://fsw62-todos-api.herokuapp.com/api/todos/4b0c7900
 ```
======================================
***Response***
{
    "payload": {
        "id": "4b0c7900",
        "owner": "Sihame",
        "text": "lab",
        "completed": true
    },
    "err": false
}
======================================
***Body***

```json
  yes with put we have to use body
  x-wwwform-urlencoded
* text: lab

```
======================================
    ***What does it do?***

```json

  PATCH  user id at the endpoint to update partial information for a specific ID

```
======================================
***status codes***

```json
status: 200ok

```
======================================
***6.DELETE  ====>/todos/<todo-id>:**
--------------------------------
***Request: METHOD - ENDPOINT***
```json
 https://fsw62-todos-api.herokuapp.com/api/todos/4b0c7900
```
======================================
***Response***

{
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}
======================================
***Body***

```json
No we don't need body

```
======================================

    ***What does it do?***

```json

  it delete user with ID

```
======================================
***status codes***

```json
status: 404ok

```
======================================

2. Find as much status codes as possible. I will tell you how many there are by the end.
we have 3 status codes:
200 ok,201 created, and 404 not found, 

