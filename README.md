# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint                 | 
|--------|--------------------------|
| `GET`  | `/users`                 |
| `GET`  | `/users/<user-username>` |
| `POST` | `/users/signup`          |

#### Todos
| Method   | Endpoint           | Possible Query Params |
|----------|--------------------|-----------------------|
| `GET`    | `/todos`           | `username=<username>`, `completed=<true\|false>`
| `POST`   | `/todos`           ||
| `GET`    | `/todos/<todo-id>` ||
| `PUT`    | `/todos/<todo-id>` ||
| `PATCH`  | `/todos/<todo-id>` ||
| `DELETE` | `/todos/<todo-id>` ||

## Tasks
1. Try out all the requests that are possible with this API. For all the possible requests create a list like the following.
Separate requests by a long line of underscores.
    * **Request**: METHOD - ENDPOINT
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      {
        "owner": "alejo4373",
        "text": "1st Todo"
      }
    ```
    * **Response**:
    ```json
    {
      "userId": 1,
      "id": 1,
      "title": "delectus aut autem",
      "completed": false
    }
    ```
    * **What does it do?**: EXPLAIN WHAT THE REQUEST DID/DO IN PLAIN ENGLISH

Question 1 ________________________________
{
    "payload": {
        "msg": "Username not available. Please try a different one."
    },
    "err": true
}

//Question 2_______________________________
    {
    "payload": {
        "id": 29,
        "username": "RougeLight"
    },
    "err": false
}
Question 3 _________________________________
Question 4__________________________________
{
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}
Question 5___________________________________
{
    "payload": {
        "id": "6bf82310",
        "owner": "RougeLight",
        "text": "I'm tide",
        "completed": false
    },
    "err": false
}
Question 6____________________________________
{
    "payload": {
        "id": "6bf82310",
        "owner": "RougeLight",
        "text": "I'm tide",
        "completed": false
    },
    "err": false
}
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
        {
            "id": 29,
            "username": "RougeLight"
}
    ],
    what does it do: gets all availible users 

2. request: GET https://fsw62-todos-api.herokuapp.com/api/users/sunnyd
body: empty
repspose:
{
    "payload": {
        "id": 26,
        "username": "sunnyd"
    },
    "err": false
}
    what does it do: gets info about user sunnyd
3. request:
POST https://fsw62-todos-api.herokuapp.com/api/users/signup

body:
{
    username:hitch
}

response:
{
    "payload": {
        "user": {
            "id": 45,
            "username": "hitch"
        },
        "msg": "User created"
    },
    "err": false
}
    what does it do: creates a new user by the name of hitch
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
    ]
    "err": false
}
    what does it do: gets all todos
5. request:
POST https://fsw62-todos-api.herokuapp.com/api/todos

body:{
    owner: "RougeLight"
    text: "This lab for the Dev plan"
}

response:
{
    "payload": {
        "id": "dee709e0",
        "owner": "RougeLight",
        "text": "This lab for the Dev Plan",
        "completed": false
    },
    "err": false
}
    what does it do: creates a new todo
2. Find as much status codes as possible. I will tell you how many there are by the end.


### Bonuses
1. Take a look at the next lesson to learn how to make make network requests with Javascript.
Since you previously had build a simple Todos App with HTML and now you know how to manipulate
the DOM, add some JS to try to connect that app to this API so that todos you enter in the page 
are saved to the API. Marking a todo as complete or uncompleted should work.
2. Find the easter egg.
