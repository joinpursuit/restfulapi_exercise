# Users Q1
**Request**: GET - https://fsw62-todos-api.herokuapp.com/api/users
**Body**: No body because no keys and values were used. 

**Response**:
  {
    "payload": [
        {
            "id": 1,
            "username": "
        },alejo4373"
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
        }
    ],
    "err": false
}
**Explanation**: The request its accessing the Heroku app database and its getting the API of all the users. The endpoint in return its providing all the users' id and username. 

#Q2 
**Request**: GET- https://fsw62-todos-api.herokuapp.com/api/users/alejo4373

**Body**:No body because no keys and values were used. 
**Response**:
{
    "payload": {
        "id": 1,
        "username": "alejo4373"
    },
    "err": false
}
**Explanation**:The request its accessing the Heroku app database and its getting the API of one user. The endpoint in return its providing the one user id and username.  


#Q3 
**Request**:POST-  https://fsw62-todos-api.herokuapp.com/api/users/signup
**Body**: KEY-username Value -steph
**Response**: {
    "payload": {
        "user": {
            "id": 50,
            "username": "steph"
        },
        "msg": "User created"
    },
    "err": false
}
**Explanation**:
The request its accessing the Heroku app database and its adding (signing up) to the API one user name with the username "steph". 


# Todos Q1 
**Request**: https://fsw62-todos-api.herokuapp.com/api/todos?owner=NewNew&completed=false 
 **Body**: 
KEY-owner     Value- NewNew
KEY-completed Value-false
 **Response**: 
 {
    "payload": [
        {
            "id": "a3d4d7d0",
            "owner": "NewNew",
            "text": "Feed me Seymour! No seriously put dishes in me...",
            "completed": false
        }
    ],
    "err": false
}
 **Explanation**:
 This is providing the information of one username called "NewNew" and everything that this user completed that turns out to be "false." 

#Q2
 **Request**:
 https://fsw62-todos-api.herokuapp.com/api/todos?owner =steph&text=Supercalifragilisticexpialidocious 
 
 **Body**: key- owner  value-steph
 key- text  value- Supercalifragilisticexpialidocious
   
 **Response**: 
 {
    "payload": {
        "id": "6cb4e360",
        "owner": "steph",
        "text": "Supercalifragilisticexpialidocious ",
        "completed": false
    },
    "err": false
}
 **Explanation**:
 This is adding to the API a new owner name "steph" and text that reads "Supercalifragilisticexpialidocious."

#Task Q3
**Request**: 
https://fsw62-todos-api.herokuapp.com/api/todos/6cb4e360
**Body**: no

**Response**: 
{
    "payload": {
        "id": "6cb4e360",
        "owner": "steph",
        "text": "Supercalifragilisticexpialidocious ",
        "completed": false
    },
    "err": false
}
**Explanation**:
This is getting the user with the id number 6cb4e360.


#Q4 
**Request**:
https://fsw62-todos-api.herokuapp.com/api/todos/a3d4d7d0
 **Body**: none 
 **Response**: 
 {
    "payload": {
        "id": "a3d4d7d0",
        "owner": "steph",
        "text": "I just replaced this",
        "completed": true
    },
    "err": false
}
 **Explanation**:
This is updating all the information for user id. 

#Q5
**Request**: https://fsw62-todos-api.herokuapp.com/api/todos/a3d4d7d0
**Body**: yes 
 "id": "a3d4d7d0",
        "owner": "steph",
        "text": "its okay",
        "completed": true
**Response**: This is updating all the information for user id. 
{
    "payload": {
        "id": "a3d4d7d0",
        "owner": "steph",
        "text": "its okay",
        "completed": true
    },
    "err": false
}
**Explanation**: This is updating a specific part of the code such as the text value from "I just replace this" to " its okay."


#Q6
**Request**: delete
https://fsw62-todos-api.herokuapp.com/api/todos/a3d4d7d0
**Body**: no, it was deleted everything 
**Response**: 
{
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}
**Explanation**:  This is deleting all the information.



2. Find as much status codes as possible. I will tell you how many there are by the end.

### Bonuses
1. Take a look at the next lesson. To learn how to make make network requests with Javascript
Since you previously had build a simple Todos APP with HTML try to connect that app to this
API so that todos you enter in the page are save to the API. Marking a todo as complete or uncompleted
should work.
2. Find the easter egg.

user:
Q1-200
Q2-200
Q3-404

todos:
Q1-200
Q2-201
Q3- 200
Q4-401
Q5-404
Q6- 404
