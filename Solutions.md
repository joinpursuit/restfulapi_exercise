# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint           | What does this do? |
|--------|--------------------|--------------------|
| `GET`  | `/users`           | `_________________`|
| `GET`  | `/users/<username>` | `_________________`|
| `POST`  | `/users/signup`   | `_________________`|


* Fill in the blanks above :arrow_up: 

#### Todos
| Method   | Endpoint           | What does this do? | Possible Query Params |
|----------|--------------------|--------------------|-----------------------|
| `GET`    | `/todos`           | `_________________`| `owner=<username>`, `completed=<true|false> `
| `POST`   | `/todos`           | `_________________`||
| `GET`    | `/todos/<todo-id>` | `_________________`||
| `PUT`    | `/todos/<todo-id>` | `_________________`||
| `PATCH`  | `/todos/<todo-id>` | `_________________`||
| `DELETE` | `/todos/<todo-id>` | `_________________`||

* Fill in the blanks above :arrow_up: 

## Tasks
1. Try out all the requests that are possible with this API. For all the possible requests Create a list like the following.
Separate requests by a long line of underscores.
    * **Request**: POST - /users/signup	
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      username:Khan
    ```
    * **Response**:
    ```json
    {
    "payload": {
        "user": {
            "id": 31,
            "username": "Khan"
        },
        "msg": "User created"
    },
    "err": false
    }
    ```
    * **What does it do?**: Creates a new user.
=============================================================================== 
    * **Request**: GET - /users
    * **Body** (if applicable POST/PUT/PATCH)
    * **Response**:
    ```json
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
        }
    ],
    "err": false
}
    ```
    * **What does it do?**: Gives the list of all users (with their ids).
=============================================================================== 
    * **Request**: GET - /users/Khan
    * **Body** (if applicable POST/PUT/PATCH)
    * **Response**:
    ```json
      {
        "payload": {
          "id": 31,
          "username": "Khan"
        },
        "err": false
      }
    ```
    * **What does it do?**: Gives the specified user with his/her id.
=============================================================================== 
    * **Request**: GET - /todos
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
    {
      completed:true
    }
    ```
    * **Response**:
    ```json
    {
    "payload": [
        {
            "id": "188b0300",
            "owner": "the real not alejo4373",
            "text": "rip out hair after multiple GET errors",
            "completed": false
        },
        {
            "id": "8ed59cf0",
            "owner": "Jonezy",
            "text": "Read a book",
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
            "id": "ac30a0d0",
            "owner": "alejo4373",
            "text": "hide birth certificate",
            "completed": false
        },
        {
            "id": "deb4cb60",
            "owner": "alejo4373",
            "text": "Alejandro - Lady Gaga",
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
            "text": "(^_^)",
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
            "text": "(^_^)",
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
            "id": "2f87c0f0",
            "owner": "alejo4373",
            "text": "Alejandro - Lady Gaga",
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
            "id": "877c4830",
            "owner": "alejo4373",
            "text": "1st Todo",
            "completed": false
        },
        {
            "id": "2934e5d0",
            "owner": "alejo4373",
            "text": "nah, nah, nah",
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
        },
        {
            "id": "3dbcab80",
            "owner": "alejo4373",
            "text": "1st Todo",
            "completed": false
        }
    ],
    "err": false
}
    
    ```
    * **What does it do?**: Gives a list of all the todos stored in the server.
=============================================================================== 
    * **Request**: POST - /todos
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      //id:31
      owner:Khan
      completed:false
      text: Go to sleep
    ```
    * **Response**:
    ```json
    {
      "payload": {
        "id": "fa719550",
        "owner": "Khan",
        "text": "Go to sleep",
        "completed": false
      },
      "err": false
    }
    ```
    * **What does it do?**: Created a new todo under the user Khan
=============================================================================== 
    * **Request**: GET - /todos//fa719550
    * **Body** (if applicable POST/PUT/PATCH)
    * **Response**:
    ```json
    {
      "payload": {
        "id": "fa719550",
        "owner": "Khan",
        "text": "Go to sleep",
        "completed": false
      },
      "err": false
    }
    ```
    * **What does it do?**: Gives the todo what the id was specified on the request
=============================================================================== 
    * **Request**: PUT - /todos/fa719550
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      //id:31
      owner:Khan
      completed:false
      text:Go to sleep. Again
    ```
    * **Response**:
    ```json
    {
      "payload": {
        "id": "fa719550",
        "owner": "Khan",
        "text": "Go to sleep. Again",
        "completed": false
      },
      "err": false
    }
    ```
    * **What does it do?**: Updates the todo which the id was on the request (
      all key/values must be inclued on the request)
=============================================================================== 
    * **Request**: PATCH - /todos/fa719550
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      //id:31
      text:Go to sleep. Again. And again
    ```
    * **Response**:
    ```json
    {
      "payload": {
        "id": "fa719550",
        "owner": "A",
        "text": "Go to sleep. Again. And again",
        "completed": false
      },
      "err": false
    }
    ```
    * **What does it do?**: Updates the todo which the id was on the request with the key/value provided
=============================================================================== 
    * **Request**: DELETE - /todos/fa719550
    * **Body** (if applicable POST/PUT/PATCH)
    * **Response**:
    ```json
    {
      "payload" {
        "id": "fa719550" ,
        "owner": "Khan" ,
        "text: "Go to sleep. Again. And again" ,
        "completed": false
      },
      "err": "false"
    }
    ```
    * **What does it do?**: Delete the todo which the id was on the request.
===============================================================================   
2. Find as much status codes as possible. I will tell you how many there are by the end.
  * **201 created**: when creating a new user/todo
  * **200 OK**: for all other working requests
  * **404 not found**: for bad endopoints
  * **400 Bad request**: when trying to add a new todo but put key: username instead of owner or not all values are included
  * **409 conflict**: when trying to create a new user with a username already existing.
  * **500 Internal Server Error**: when trying to patch the id of my todo or when creating a new todo with an id that already exists.


### Bonuses
1. Take a look at the next lesson. To learn how to make make network requests with Javascript
Since you previously had build a simple Todos APP with HTML try to connect that app to this
API so that todos you enter in the page are save to the API. Marking a todo as complete or uncompleted
should work.
2. Find the easter egg.
