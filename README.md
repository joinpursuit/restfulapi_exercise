# Interacting with APIs - Exercises 

In this exercises you will be retrieving information to an API as well as adding information for the API to save. By doing this exercises you will practice and reinforce.
* HTTP Methods
* The use of URL Query Parameters to filter results
* Making network requests with Postman or `curl`
* Learn about HTTP status codes

##  Todos API
### Root Endpoint https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint            |
| ------ | ------------------- |
| `GET`  | `/users`            |
| `GET`  | `/users/<username>` |
| `POST` | `/users/signup`     |

#### Todos
| Method   | Endpoint           | Possible Query Params   |
| -------- | ------------------ | ----------------------- |
| `GET`    | `/todos`           | `username`, `completed` |
| `POST`   | `/todos`           |                         |
| `GET`    | `/todos/<todo-id>` |                         |
| `PUT`    | `/todos/<todo-id>` |                         |
| `PATCH`  | `/todos/<todo-id>` |                         |
| `DELETE` | `/todos/<todo-id>` |                         |

##### Query Params Values
* `username`: A username that exists in the API that todos are associated with.
* `completed`: A boolean `true` or `false` specifying whether the todos that are returned have been completed or not.

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

2. Find as much status codes as possible. I will tell you how many there are by the end.

### Bonuses
1. Take a look at the next lesson to learn how to make make network requests with Javascript.
Since you previously had build a simple Todos App with HTML and now you know how to manipulate
the DOM, add some JS to try to connect that app to this API so that todos you enter in the page 
are saved to the API. Marking a todo as complete or uncompleted should work.
2. Find the easter egg.
