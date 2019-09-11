# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint           | What does this do? |
|--------|--------------------|--------------------|
| `GET`  | `/users`           |`_________________`|
| `GET`  | `/users/<user-username>` |`_________________`|
| `POST`  | `/users/signup`   |`_________________`|


* Fill in the blanks above :arrow_up: 

#### Todos
| Method   | Endpoint           | What does this do? | Possible Query Params |
|----------|--------------------|--------------------|-----------------------|
| `GET`    | `/todos`           | `_________________`| `username=<username>`, `completed=<true|false> `
| `POST`   | `/todos`           | `_________________`||
| `GET`    | `/todos/<todo-id>` | `_________________`||
| `PUT`    | `/todos/<todo-id>` | `_________________`||
| `PATCH`  | `/todos/<todo-id>` | `_________________`||
| `DELETE` | `/todos/<todo-id>` | `_________________`||

* Fill in the blanks above :arrow_up: 

## Tasks
1. Try out all the requests that are possible with this API. For all the possible requests Create a list like the following.
Separate requests by a long line of underscores.
    * **Request**: METHOD - ENDPOINT
    ```json
    get (users): "https://fsw62-todos-api.herokuapp.com/api/users"
    ```
    ```json
    get(username): "https://fsw62-todos-api.herokuapp.com/api/users/alejo4373"
    ```
    * **Body** (if applicable POST/PUT/PATCH)
    ```json
      <!-- {
        "owner": "alejo4373",
        "text": "1st Todo"
      } -->
      ```
      
      ```json
      Get: has no body.
      ```

  
    * **Response**:
    ```json
    <!-- {
      "userId": 1,
      "id": 1,
      "title": "delectus aut autem",
      "completed": false
    } -->
      ```
      
  get (users): {
    "payload": [
        {
            "id": 1,
            "username": "alejo4373"
        },
        {
            "id": 2,
            "username": "JRJRocks"
        }
    ```
    ```json
    get (username): {
    "payload": {
        "id": 1,
        "username": "alejo4373"
    },
    "err": false
}
 ```

    * **What does it do?**: EXPLAIN WHAT THE REQUEST DID/DO IN PLAIN ENGLISH
  ```json
The GET request for the users gives you the object list of the users in an array. 
  ```

  ```json
    The GET request for the username allows you to get the info of one username.
  ```

2. Find as much status codes as possible. I will tell you how many there are by the end.

### Bonuses
1. Take a look at the next lesson. To learn how to make make network requests with Javascript
Since you previously had build a simple Todos APP with HTML try to connect that app to this
API so that todos you enter in the page are save to the API. Marking a todo as complete or uncompleted
should work.
2. Find the easter egg.
