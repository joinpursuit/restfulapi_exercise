# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint           | What does this do? |
|--------|--------------------|--------------------|
| `GET`  | `/users`           | `Gives a list of users`|
| `GET`  | `/users/<user-id>` | `This gives us a specific user`|
| `POST`  | `/users/signup`   | `A new user with the usename that I entered`|


* Fill in the blanks above :arrow_up: 

#### Todos
| Method   | Endpoint           | What does this do? | Possible Query Params |
|----------|--------------------|--------------------|-----------------------|
| `GET`    | `/todos`           | `A list of to do items created by a user`| `username=<username>`, `completed=<true|false> `
| `POST`   | `/todos`           | `This creates a todos list item for a user`||
| `GET`    | `/todos/<todo-id>` | `This gives gives a todo item based on the id entered`||
| `PUT`    | `/todos/<todo-id>` | `gives the ability to change all of the values in the file`||
| `PATCH`  | `/todos/<todo-id>` | `Changes a specific value in the file`||
| `DELETE` | `/todos/<todo-id>` | `Deleted the todo list file`||

* Fill in the blanks above :arrow_up: 

## Tasks
1. Try out all the requests that are possible with this API. For all the possible requests Create a list like the following.
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

2. Find as much status codes as possible. I will tell you how many there are by the end.

### Bonuses
1. Take a look at the next lesson. To learn how to make make network requests with Javascript
Since you previously had build a simple Todos APP with HTML try to connect that app to this
API so that todos you enter in the page are save to the API. Marking a todo as complete or uncompleted
should work.
2. Find the easter egg.
