1.
request: GET https://fsw62-todos-api.herokuapp.com/api/users
body: empty
repspose:
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
    what does it do: gets all availible users 
    ________________________________________________________________________________________________
2. request: GET https://fsw62-todos-api.herokuapp.com/api/users/pecan_breezy
body: empty
repspose:
{
    "payload": {
        "id": 27,
        "username": "pecan_breezy"
    },
    "err": false
}
    what does it do: gets info about user pecan_breezy
____________________________________________________________________________________________________

3. request:
POST https://fsw62-todos-api.herokuapp.com/api/users/signup

body:
{
    username:prncessbri94
}

response:
{
    "payload": {
        "user": {
            "id": 37,
            "username": "prncessbri94"
        },
        "msg": "User created"
    },
    "err": false
}
    what does it do: creates a new user by the name of prncessbri94
____________________________________________________________________________________________________

4. request:
GET https://fsw62-todos-api.herokuapp.com/api/todos

body: empty

response:
{
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
        },
        {
            "id": "340548e0",
            "owner": "fullStackGuy",
            "text": "clean up 6.1's mess",
            "completed": false
        },
        {
            "id": "776f95e0",
            "owner": "fullStackGuy",
            "text": " worry about whether or not I really understand what's going on",
            "completed": false
        }
    ],7
    "err": false
}
    what does it do: gets all availible todos
____________________________________________________________________________________________________
5. request:
POST https://fsw62-todos-api.herokuapp.com/api/todos

body:{
    owner:prncessbri94
    text: follow me on IG :)
}

response:
{
    "payload": {
        "id": "faeaaf30",
        "owner": "prncessbri94",
        "text": " follow me on IG :)",
        "completed": false
    },
    "err": false
}
    what does it do: creates a new todo
____________________________________________________________________________________________________

6. request:
GET https://fsw62-todos-api.herokuapp.com/api/todos/9dc725e0

body:

response:
{
    "payload": {
        "id": "9dc725e0",
        "owner": "sunnyd",
        "text": "Deja actually hates sunny D",
        "completed": false
    },
    "err": false
}
    what does it do: gets a specific todo based on user
____________________________________________________________________________________________________
7. request:
PUT https://fsw62-todos-api.herokuapp.com/api/todos/prncessbri94

body:
    id:prncessbri94
    owner:prncessbri94
    text:hope ya'll are having fun
    completed:true

response:
{
    "payload": {
        "id": "prncessbri94",
        "owner": "prncessbri94",
        "text": "hope ya'll are having fun",
        "completed": true
    },
    "err": false
}

    what does it do: updates the user's post
____________________________________________________________________________________________________

8. request:
PATCH https://fsw62-todos-api.herokuapp.com/api/todos/0d0fce60

body:
    {
        text: tiredddddddddd
    }

response:
{
    "payload": {
        "id": "0d0fce60",
        "owner": "pecan_breezy",
        "text": " tiredddddddddd",
        "completed": true
    },
    "err": false
}

    what does it do: updates the user's post
____________________________________________________________________________________________________
9. request:
DELETE https://fsw62-todos-api.herokuapp.com/api/todos/prncessbri94

body:empty

response:
{
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}

    what does it do: removes the todo from a specific user
____________________________________________________________________________________________________
