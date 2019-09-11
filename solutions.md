https://fsw62-todos-api.herokuapp.com/api

1. GET USERS
```
* Request: GET https://fsw62-todos-api.herokuapp.com/api/users
* Body: None
* Request: {
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
        }
    ],
    "err": false
}
```
____________________________________________________________________________________________________
This method returns a collection of all the users in herokuapp. There is no body to a GET method

2. GET Users/<username>
```
* Request: GET https://fsw62-todos-api.herokuapp.com/api/users/JRJRocks
* Body: None
* Reponse: {
    "payload": {
        "id": 2,
        "username": "JRJRocks"
    },
    "err": false
}
```
_________________________________________________________________________________________________________
This method return a specific (one) user data from the herokuapp. There is no body to a GET method

3. POST users/signup
```
* Request: POST https://fsw62-todos-api.herokuapp.com/api/users/signup
* Body: username:kitkatjewels
* Response: None
```
___________________________________________________________________________________________________________
There is no response to this method. It simply create a new user to the herokuapp

4. GET /todos
```
 * Request: GET https://fsw62-todos-api.herokuapp.com/api/todos
 * Body: NONE
 * Response: {
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
            "id": "666",
            "owner": "Cow",
            "text": "Moo some more",
            "completed": false
        }
```
________________________________________________________________________________________________________________________
Return all the todos from the herokuapp.

5. POST /todos
```
* Request: POST https://fsw62-todos-api.herokuapp.com/api/todos
* Body:  //username:kitkatjewels
           owner:kitkatjewels
           text:I am sleepy!
           //completed:
* Response: None
```
_________________________________________________________________________________________________________________________
added a text value for the owner kitkatjewels

6. GET /todos/<todo-id> 
```
* Request: GET https://fsw62-todos-api.herokuapp.com/api/todos/0d0fce60
* Body: None
* Response: 
{
    "payload": {
        "id": "0d0fce60",
        "owner": "kitkatjewels",
        "text": "I am sleepy!",
        "completed": false
    },
    "err": false
```
____________________________________________________________________________________________________________________________

7. PUT todos/<todo-id>
```
* Request: PUT https://fsw62-todos-api.herokuapp.com/api/todos/0d0fce60
* Body: //username:kitkatjewels
          owner:kitkatjewels
          text:I am awake now!
          completed:true
* Response: 
```
{
    "payload": {
        "id": "0d0fce60",
        "owner": "kitkatjewels",
        "text": "I am awake now!",
        "completed": true
    },
    "err": false
}
____________________________________________________________________________________________________________________________
updates the todo data for kitkatjewels from being sleepy to being awake. Also the completed field from false to true.

8. PATCH todos/<todo-id>
```
* Request: PATCH https://fsw62-todos-api.herokuapp.com/api/todos/0d0fce60
* Body: text:is NEVER tired
* Response: 
  {
    "payload": {
        "id": "0d0fce60",
        "owner": "pecan_breezy",
        "text": "is NEVER tired",
        "completed": true
    },
    "err": false
}
```
____________________________________________________________________________________________________________________________
partially changes data from the todo rather the entire todo 

9. DELETE todos/<todo-id>
```
* Request: DELETE https://fsw62-todos-api.herokuapp.com/api/todos/0d0fce60
* Body: No body
* Response: 
    {
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}
```
___________________________________________________________________________________________________________________________
removes the todo from a specific user