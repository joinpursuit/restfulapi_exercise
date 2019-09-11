##Task One

## One
* **Request**: `GET` - `/users`
* **Body**
```json

```
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
        }
    ],
    "err": false
}
```
* **What does it do?**: The method GET is displaying all the users that have been stored in the API with the parameter or endpoint '/users'.
__________________________________________________________________________
## Two
* **Request**: `GET` - `/users/Run%20The%20Jewels`
* **Body**
```json

```
* **Response**:
```json
{
    "payload": {
        "id": 24,
        "username": "Run The Jewels"
    },
    "err": false
}
```
* **What does it do?**: The method GET is displaying one user who is hardcoded into the endpoint and all its details
__________________________________________________________________________
## Three
* **Request**: `POST` - `/users/signup`
* **Body**
```json
  {
    "username": "Dish Washing Monster"
  }
```
* **Response**:
```json
{
    "payload": {
        "user": {
            "id": 55,
            "username": "Dish Washing Monster"
        },
        "msg": "User created"
    },
    "err": false
}
```
* **What does it do?**: The method POST method is using the signup Endpoint to add new records to the API list that is actually working. The whole class is adding stuff
__________________________________________________________________________
## Four
* **Request**: `GET` - `/todos`
* **Body**
```json

```
* **Response**:
```json
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
            "id": "83f01010",
            "owner": "Stink Meaner",
            "text": "Fight Robert Freedman",
            "completed": true
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
            "id": "a63aade0",
            "owner": " theRealObama",
            "text": "squish",
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
            "id": "31786e60",
            "owner": "Mike923",
            "text": "found who did it ",
            "completed": true
        }
    ],
    "err": false
}
```
* **What does it do?**: 
__________________________________________________________________________
## Five
* **Request**: `POST` - `/todos`
* **Body**
```json
        "owner": "Dish Washing Monster",
        "text": "Feed me Seymour! No seriously put dishes in me...",
```
* **Response**:
```json
{
    "payload": {
        "id": "81ba6a60",
        "owner": "Dish Washing Monster",
        "text": "Feed me Seymour! No seriously put dishes in me...",
        "completed": false
    },
    "err": false
}
```
* **What does it do?**: The POST method is creating the todo list with the user name
__________________________________________________________________________
## Six
* **Request**: `GET` - `https://fsw62-todos-api.herokuapp.com/api/todos/81ba6a60`
* **Body**
```json

```
* **Response**:
```json
{
    "payload": {
        "id": "81ba6a60",
        "owner": "Dish Washing Monster",
        "text": "Feed me Seymour! No seriously put dishes in me...",
        "completed": false
    },
    "err": false
}
```
* **What does it do?**: With this GET method pointed at the id of the todo list we just created we can get all the data from it
__________________________________________________________________________
## Seven
* **Request**: `PUT` - `https://fsw62-todos-api.herokuapp.com/api/todos/81ba6a60`
* **Body**
```json
    "owner" : "Dish Washing Monster"
    "text" : "Is this finished yet?"
    "completed" : false
```
* **Response**:
```json
{
    "payload": {
        "id": "81ba6a60",
        "owner": "Dish Washing Monster",
        "text": "Is this finished yet?",
        "completed": false
    },
    "err": false
}
```
* **What does it do?**: The PUT method allows me to change the text and completed keys but I have to change them both at once. I can add entire new information here that overwrites the old or just add a new text and completed.
__________________________________________________________________________
## Eight
* **Request**: `PATCH` - `https://fsw62-todos-api.herokuapp.com/api/todos/81ba6a60`
* **Body**
```json
    "text" : "Feed me Seymour! No seriously put dishes in me..."
```
* **Response**:
```json
{
    "payload": {
        "id": "81ba6a60",
        "owner": "Dish Washing Monster",
        "text": "Feed me Seymour! No seriously put dishes in me...",
        "completed": false
    },
    "err": false
}
```
* **What does it do?**: With PATCH I can modifiy one text line
__________________________________________________________________________
## Nine
* **Request**: `DELETE` - `https://fsw62-todos-api.herokuapp.com/api/todos/83f01010`
* **Body**
```json

```
* **Response**:
```json
        {
            "id": "83f01010",
            "owner": "Stink Meaner",
            "text": "died, I shall return even meaner",
            "completed": true
        }
```
* **What does it do?**: This method DELETES a whole todo record completely

## Task Two

* **Status Codes**:
200 (OK HTTPS Repsonse)
400 (Bad Request)
404 (Not Found)


