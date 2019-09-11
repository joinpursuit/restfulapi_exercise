1. ######USERS######
GET Users:
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
        }
        ],
        "err": false
    }  

  Posts all user ids and names      
________________________________________________________________________________

GET  | /users/<user-id>:

{
    "payload": {
        "id": 49,
        "username": "GetSchwifty"
    },
    "err": false
}
 post unique user
________________________________________________________________________________

POST  | /users/signup:

{
"id": 49,
"username": "GetSchwifty"
}

creates a new user

########TODOS#######

GET    | /todos
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
        }
        ],
        "err": false
    }
    posts all users todos

________________________________________________________________________________

POST   | /todos

{
    "payload": {
        "id": "7f101cd0",
        "owner": "GetSchwifty",
        "text": "BBQ pizza sucks",
        "completed": false
    },
    "err": false
}

post unique todo

________________________________________________________________________________

GET    | /todos/<todo-id>

{
    "payload": {
        "id": "5ebb70b0",
        "owner": "GetSchwifty",
        "text": "BBQ pizza sucks",
        "completed": false
    },
    "err": false
}
get the unique user
________________________________________________________________________________

PUT    | /todos/<todo-id>

{
    "payload": {
        "id": "5ebb70b0",
        "owner": "GetSchwifty",
        "text": "BBQ pizza sucks",
        "completed": true
    },
    "err": false
}

add a different text

________________________________________________________________________________

PATCH  | /todos/<todo-id>
{
    "payload": {
        "id": "5ebb70b0",
        "owner": "GetSchwifty",
        "text": "pineapple pizza next time",
        "completed": true
    },
    "err": false
}
modifies the text

________________________________________________________________________________

DELETE | /todos/<todo-id>

{
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}

deletes the user id




2. Status Codes: 200
