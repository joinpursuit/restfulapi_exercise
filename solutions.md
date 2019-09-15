1.
Request: GET - https://fsw62-todos-api.herokuapp.com/api/users
Response: {
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
        },
        {
            "id": 29,
            "username": " woah"
        },
        {
            "id": 30,
            "username": "Bernie Gang"
        },
        {
            "id": 31,
            "username": "Khan"
        },
        {
            "id": 32,
            "username": "ShaynaRocks"
        },
        {
            "id": 34,
            "username": "huey"
        },
        {
            "id": 35,
            "username": "fullStackGuy"
        },
        {
            "id": 37,
            "username": "prncessbri94"
        },
        {
            "id": 38,
            "username": " savitaAnn"
        },
        {
            "id": 39,
            "username": " Aransa"
        },
        {
            "id": 40,
            "username": "Hello There!"
        },
        {
            "id": 41,
            "username": "You know whar we not gonna do"
        },
        {
            "id": 42,
            "username": "RougeLight"
        },
        {
            "id": 43,
            "username": "baconeggandcheese"
        },
        {
            "id": 45,
            "username": "test"
        },
        {
            "id": 46,
            "username": "theYoungRebel"
        },
        {
            "id": 47,
            "username": "Jonezy"
        },
        {
            "id": 48,
            "username": " potato"
        },
        {
            "id": 49,
            "username": "GetSchwifty"
        },
        {
            "id": 50,
            "username": "steph"
        },
        {
            "id": 51,
            "username": "jo"
        },
        {
            "id": 52,
            "username": "Sihame"
        },
        {
            "id": 53,
            "username": "NewNew"
        },
        {
            "id": 55,
            "username": "Dish Washing Monster"
        },
        {
            "id": 56,
            "username": "Roscoe Merryweather"
        },
        {
            "id": 59,
            "username": "test3"
        },
        {
            "id": 61,
            "username": "GrilledCheeseFan93"
        },
        {
            "id": 62,
            "username": "Kathy"
        },
        {
            "id": 64,
            "username": "Bazi"
        },
        {
            "id": 66,
            "username": "lol"
        },
        {
            "id": 67,
            "username": "KissMy_Dance"
        },
        {
            "id": 70,
            "username": "Coww"
        },
        {
            "id": 72,
            "username": "hello"
        },
        {
            "id": 75,
            "username": "1"
        },
        {
            "id": 77,
            "username": "easteregg"
        },
        {
            "id": 78,
            "username": "My"
        },
        {
            "id": 79,
            "username": "asdf"
        },
        {
            "id": 80,
            "username": "chicken"
        }
    ],
    "err": false
}
What does it do?: provides a complete list of users
____________________________________________________________
Request: GET - https://fsw62-todos-api.herokuapp.com/api/users/Mike923
Response: {
    "payload": {
        "id": 3,
        "username": "Mike923"
    },
    "err": false
}
What does it do?: provides information on a single user
___________________________________________________________________
Method: POST - https://fsw62-todos-api.herokuapp.com/api/users/signup
Body: username: Serge
Response: {
    "payload": {
        "user": {
            "id": 81,
            "username": " Serge"
        },
        "msg": "User created"
    },
    "err": false
}
What does it do?: adds a user
__________________________________________________________________________
Method: GET - https://fsw62-todos-api.herokuapp.com/api/todos
Response:{
    "payload": [
        {
            "id": "8",
            "owner": "alejo4373",
            "text": "delectus aut autem",
            "completed": true
        },
        {
            "id": "kjnwfw",
            "owner": "asdf",
            "text": "asdf",
            "completed": false
        },
        {
            "id": "1234",
            "owner": "chicken",
            "text": "Eat my friends and family",
            "completed": false
        },
        {
            "id": "134cdb40",
            "owner": "Cow",
            "text": "2nd Todo",
            "completed": false
        },
        {
            "id": "888",
            "owner": "alejo4373",
            "text": "1st Todoasdf",
            "completed": false
        },
        {
            "id": "188b0300",
            "owner": "the real not alejo4373",
            "text": "rip out hair after multiple GET errors",
            "completed": false
        },
        {
            "id": "60455f50",
            "owner": "alejo4373",
            "text": "1st Todoadklfjadfamnsdf",
            "completed": false
        },
        {
            "id": "8ed59cf0",
            "owner": "Jonezy",
            "text": "Read a book",
            "completed": false
        },
        {
            "id": "3d45cf70",
            "owner": "the real not alejo4373",
            "text": "check",
            "completed": false
        },
        {
            "id": "666",
            "owner": "Cow",
            "text": "Feed me Seymour! No seriously put dishes in me...",
            "completed": true
        },
        {
            "id": "b65b6930",
            "owner": "Stink Meaner",
            "text": "why delete",
            "completed": false
        },
        {
            "id": "1234567890",
            "owner": " Aransa",
            "text": "hola como estas? ",
            "completed": true
        },
        {
            "id": "fa719550",
            "owner": "Khan",
            "text": "Go to sleep",
            "completed": false
        },
        {
            "id": "fd3a5dd0",
            "owner": "the real not alejo4373",
            "text": "stare blankly at Postman for HOURS",
            "completed": true
        },
        {
            "id": "1a4a81c0",
            "owner": "Khan",
            "text": "Go to sleep",
            "completed": false
        },
        {
            "id": "7",
            "owner": "okurrrt",
            "text": " ummm idk what to do",
            "completed": true
        },
        {
            "id": "b47be9e0",
            "owner": "test",
            "text": "estt",
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
            "id": "7f101cd0",
            "owner": "GetSchwifty",
            "text": "BBQ pizza sucks",
            "completed": false
        },
        {
            "id": "22c3f5d0",
            "owner": "A",
            "text": "(^^)",
            "completed": false
        },
        {
            "id": "340548e0",
            "owner": "fullStackGuy",
            "text": "clean up 6.1's mess",
            "completed": false
        },
        {
            "id": "777",
            "owner": "A",
            "text": "(^^)",
            "completed": false
        },
        {
            "id": "c3c05420",
            "owner": "Cow",
            "text": "Moo some more",
            "completed": false
        },
        {
            "id": "f8e01150",
            "owner": "steph",
            "text": "its okay",
            "completed": false
        },
        {
            "id": "762238e0",
            "owner": "A pimp named slickback",
            "text": "It's hard out here for a pimp. So make it easier. ",
            "completed": false
        },
        {
            "id": "81ba6a60",
            "owner": "Dish Washing Monster",
            "text": "Feed me Seymour! No seriously put dishes in me...",
            "completed": false
        },
        {
            "id": "8a3d6540",
            "owner": "Roscoe Merryweather",
            "text": "Bust out of jail",
            "completed": true
        },
        {
            "id": "faeaaf30",
            "owner": "prncessbri94",
            "text": " follow me on IG :)",
            "completed": false
        },
        {
            "id": "5e8219a0",
            "owner": "Cow",
            "text": "Moo some more",
            "completed": false
        },
        {
            "id": "60976a60",
            "owner": "theYoungRebel",
            "text": "it's all about Queens",
            "completed": false
        },
        {
            "id": "622c0ed0",
            "owner": "Cow",
            "text": "Moo some more",
            "completed": false
        },
        {
            "id": "7b17e900",
            "owner": "Cow",
            "text": "Moo some more",
            "completed": false
        },
        {
            "id": "7c4c2340",
            "owner": "Cow",
            "text": "Moo some more",
            "completed": false
        },
        {
            "id": "6666",
            "owner": "Cow",
            "text": "Moo some more",
            "completed": false
        }
    ],
    "err": false
}
What does it do?: list of todos and their status
___________________________________________________________________
Method: POST - https://fsw62-todos-api.herokuapp.com/api/todos
Body: owner: Mike923
      text: move
Response: {
    "payload": {
        "id": "5c1e4230",
        "owner": "Mike923",
        "text": "move",
        "completed": false
    },
    "err": false
}
What does it do?: adds a task to the todo list
__________________________________________________________________________
Method: GET - https://fsw62-todos-api.herokuapp.com/api/todos/6666
Response: {
    "payload": {
        "id": "6666",
        "owner": "Cow",
        "text": "Moo some more",
        "completed": false
    },
    "err": false
}
What does it do?: info on a specific task
___________________________________________________________________
Method: PUT - https://fsw62-todos-api.herokuapp.com/api/todos/6666
Body: owner:Mike923
      text:move
      completed:true
Response: {
    "payload": {
        "id": "6666",
        "owner": "Mike923",
        "text": "move",
        "completed": true
    },
    "err": false
}
What does it do?: changes the information of a task
_________________________________________________________________
Method: PATCH - https://fsw62-todos-api.herokuapp.com/api/todos/6666
Body: completed:false
Response: {
    "payload": {
        "id": "6666",
        "owner": "Mike923",
        "text": "cow",
        "completed": false
    },
    "err": false
}
What does it do?: updates the status of as task
_________________________________________________________________
Method: DELETE - https://fsw62-todos-api.herokuapp.com/api/todos/6666
Response: {
    "payload": {
        "id": "6666",
        "owner": "Mike923",
        "text": "cow",
        "completed": false
    },
    "err": false
}
What does it do?: deletes a task

2.
200 OK
201 CREATED
404 NOT FOUND
501 SERVICE UNAVAILABLE
