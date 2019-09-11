1. Get:https://fsw62-todos-api.herokuapp.com/api/users/
 body

Request: {
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
        },
        {
            "id": 25,
            "username": "the real not alejo4373"
        },
        {
            "id": 26,
            "username": "sunnyd"
        },
        {
            "id": 27,
            "username": "pecan_breezy"
        },
        {
            "id": 28,
            "username": "kitkatjewels"
        }
    ],
    "err": false
}
  1. Get - Prints the id for all the users.
_____________________________________________________________________________________
2. get: https://fsw62-todos-api.herokuapp.com/api/users/sunnyd
body:
request: {
    "payload": {
        "id": 26,
        "username": "sunnyd"
    },
    "err": false
}
Shows the username and id
________________________________________________________________________________________
3. post: https://fsw62-todos-api.herokuapp.com/api/users/signup/
body: username:sunnyd
post up the username sunny d in the body

________________________________________________________________________________________
4. get: https://fsw62-todos-api.herokuapp.com/api/todos
body:
request: {
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
        },
        {
            "id": "969d7210",
            "owner": "Lil Thanos",
            "text": "Snap Yo Fingers! Do ya steps!",
            "completed": false
        },
        {
            "id": "188b0300",
            "owner": "the real not alejo4373",
            "text": "rip out hair after multiple GET errors",
            "completed": false
        },
        {
            "id": "2f77d8e0",
            "owner": "the real not alejo4373",
            "text": "look over at neighbor's screen to see if they're anywhere better in the lab",
            "completed": false
        },
        {
            "id": "fd3a5dd0",
            "owner": "the real not alejo4373",
            "text": "stare blankly at Postman for minutes",
            "completed": true
        },
        {
            "id": "7b453650",
            "owner": "the real not alejo4373",
            "text": "wish i had the real alejo4373's knowledge",
            "completed": false
        },
        {
            "id": "8feb0260",
            "owner": "the real not alejo4373",
            "text": "find edible food. profit!!!",
            "completed": false
        },
        {
            "id": "7",
            "owner": "okurrrt",
            "text": " ummm idk what to do",
            "completed": true
        },
        {
            "id": "ac30a0d0",
            "owner": "alejo4373",
            "text": "hide birth certificate",
            "completed": false
        },
        {
            "id": "129d9b90",
            "owner": "Bernie Gang",
            "text": "Seize the means of production and inhalation ",
            "completed": false
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
            "id": "a7a7e790",
            "owner": " woah",
            "text": " idk wtf im doing",
            "completed": false
        },
        {
            "id": "05402bb0",
            "owner": "A pimp named slickback",
            "text": "smack a hose",
            "completed": false
        }
    ],
    "err": false
}
shows the text and if it was completed
________________________________________________________________________________________
________________________________________________________________________________________
5. post: https://fsw62-todos-api.herokuapp.com/api/todos/
body:owner": "sunnyd",
        "text": "Deja actually hates sunny D"
request: {
    "payload": {
        "id": "9dc725e0",
        "owner": "sunnyd",
        "text": "Deja actually hates sunny D",
        "completed": false
    },
    "err": false
}

shows the id number, owner, text and if task completed
________________________________________________________________________________________
6. get: https://fsw62-todos-api.herokuapp.com/api/todos/9dc725e0
body:owner": "sunnyd",
        "text": "Deja actually hates sunny D"
request: {
    "payload": {
        "id": "9dc725e0",
        "owner": "sunnyd",
        "text": "Deja actually hates sunny D",
        "completed": false
    },
    "err": false
}

shows the id number, owner, text and if task completed
________________________________________________________________________________________
7. put: https://fsw62-todos-api.herokuapp.com/api/todos/9dc725e0
body:"owner": "sunnyd",
        "text": "Deja actually hates sunny D and hawaiian punch",
        "completed": true
repest:{
    "payload": {
        "id": "9dc725e0",
        "owner": "sunnyd",
        "text": "Deja actually hates sunny D and hawaiian punch",
        "completed": true
    },
    "err": false
}
added to the request
________________________________________________________________________________________
8. patch: https://fsw62-todos-api.herokuapp.com/api/todos/9dc725e0
body:"owner": "kitkatjewels",
        "text": "Deja actually hates sunny D and hawaiian punch but loves agave juice ",
        "completed": true
{
    "payload": {
        "id": "9dc725e0",
        "owner": "kitkatjewels",
        "text": "Deja actually hates sunny D and hawaiian punch but loves agave juice ",
        "completed": false
    },
    "err": false
}
changed the owner but not the whole request
________________________________________________________________________________________
9. delete: https://fsw62-todos-api.herokuapp.com/api/todos/9dc725e0
request:{
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}
deletes the todo