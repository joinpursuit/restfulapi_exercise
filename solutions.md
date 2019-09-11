GET users 

Request : get (users): "https://fsw62-todos-api.herokuapp.com/api/users"

Body: No body for GET.

response:  {
    "payload": [
        {
            "id": 1,
            "username": "alejo4373"
        },
        {
            "id": 2,
            "username": "JRJRocks"
        }
    ]
}

What does it do?
 The GET request for the users gives you the object list of the users and their ids in an array.


GET Username 

Request: "https://fsw62-todos-api.herokuapp.com/api/users/alejo4373"

Body: Get doesn't have a body. 

Response:   get (username): {
    "payload": {
        "id": 1,
        "username": "alejo4373"
    },
    "err": false
}

What does it do? The GET request for the username allows you to get the info of one username.


POST Signup

Request: 
"https://fsw62-todos-api.herokuapp.com/api/users/signup"

Body: (username: jo)

Response: post (signup) {
    "payload": {
        "user": {
            "id": 51,
            "username": "jo"
        },
        "msg": "User created"
    },
    "err": false
}

What does it do? It creates a new user 


PART2

GET Todos

Request: "https://fsw62-todos-api.herokuapp.com/api/todos"

Getting one todos for username/ complete true

"https://fsw62-todos-api.herokuapp.com/api/todos?completed=true"

"https://fsw62-todos-api.herokuapp.com/api/todos?owner=NewNew"





Body: none

Response: {
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
        
    ],
"err": false
}

Getting one todos.
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
            "id": "7b453650",
            "owner": "the real not alejo4373",
            "text": "wish i had the real alejo4373's knowledge",
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
            "id": "83f01010",
            "owner": "Stink Meaner",
            "text": "died, I shall return even meaner",
            "completed": true
        },
        {
            "id": "5b26e2d0",
            "owner": "baconeggandcheese",
            "text": "two word",
            "completed": true
        }
    ],
    "err": false
}


POST Todos

Request: "https://fsw62-todos-api.herokuapp.com/api/todos"

Body: (id :1234567890
owner:jo
text:APIs?
completed :false)

Resource: {
    "payload": {
        "id": "e5fbdd20",
        "owner": "jo",
        "text": "APIs?",
        "completed": false
    },
    "err": false
}


GET Todos Id

https://fsw62-todos-api.herokuapp.com/api/todos/e5fbdd20


{
    "payload": {
        "id": "e5fbdd20",
        "owner": "jo",
        "text": "APIs?",
        "completed": false
    },
    "err": false
}

PUT Todos Id

https://fsw62-todos-api.herokuapp.com/api/todos/e5fbdd20

{
    "payload": {
        "id": "e5fbdd20",
        "owner": "jo",
        "text": "APIs?",
        "completed": true
    },
    "err": false
}

PATCH Todos Ids

https://fsw62-todos-api.herokuapp.com/api/todos/e5fbdd20

{
    "payload": {
        "id": "e5fbdd20",
        "owner": "jo",
        "text": "hi",
        "completed": true
    },
    "err": false
}

DELETE Todos Ids

https://fsw62-todos-api.herokuapp.com/api/todos/e5fbdd20

{
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}