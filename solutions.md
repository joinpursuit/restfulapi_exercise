# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint           | What does this do?                                                                            |
|--------|--------------------|--------------------                                                                           |
| `GET`  | `/users`           | `Read information staring from the endpoint users:Get an array of all the ids and usernames`  |
| `GET`  | `/users/<user-id>` | `Read informations starting from a specific endpoint of a specific user id and their username`|
| `POST`  | `/users/signup`   | `Create a new Id`                                                                             |


* Fill in the blanks above :arrow_up:

#### Todos
| Method   | Endpoint           | What does this do?                            | Possible Query Params    |
|----------|--------------------|-----------------------------------------------|-----------------------   |
| `GET`    | `/todos`           | `Read from the endpoint todos`                | `username=<username>`, `completed=<true|false> `
| `POST`   | `/todos`           | `Add a new todos`                             ||
| `GET`    | `/todos/<todo-id>` | `Read information on the specific id`         ||
| `PUT`    | `/todos/<todo-id>` | `Update all info in the specific user id.    `||
| `PATCH`  | `/todos/<todo-id>` | `Update partial info for the specific user id`||
| `DELETE` | `/todos/<todo-id>` | `Delete the info of the specific user id`     ||



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



**Request**:
```
{
  "id": 62,
  "username": "Kathy"
}

```

**Request**:PUT/todos/<todo-id>
**Body**:
```json
{
    "payload": {
        "id": "5b26e2d0",
        "owner": "baconeggandcheese",
        "text": "one word",
        "completed": false
    },
    "err": false
}
```
**Response**:Update all info in the specific user id.
```json
{
    "payload": {
        "id": "5b26e2d0",
        "owner": "baconeggandcheese",
        "text": "two words",
        "completed": true
    },
    "err": false
}
```



**Request**:PATCH /todos/<todo-id>
**Body**:
```json
{
    "payload": {
        "id": "5b26e2d0",
        "owner": "baconeggandcheese",
        "text": "one word",
        "completed": false
    },
    "err": false
}
```
**Response**:Update partial info for the specific user id
```json
{
    "payload": {
        "id": "5b26e2d0",
        "owner": "baconeggandcheese",
        "text": "one word",
        "completed": true
    },
    "err": false
}
```





2. Find as much status codes as possible. I will tell you how many there are by the end.

### Bonuses
1. Take a look at the next lesson. To learn how to make make network requests with Javascript
Since you previously had build a simple Todos APP with HTML try to connect that app to this
API so that todos you enter in the page are save to the API. Marking a todo as complete or uncompleted
should work.
2. Find the easter egg.







# RESTful API Practice

Create a README (`.md`) file and paste all of the responses from the server for each request. Utilize the [JSON Placeholder API](https://jsonplaceholder.typicode.com/) for each request.

1.  Send a `GET` request to the route `/users` to get the user with the `id` 7.
{
  "id": 7,
  "name": "Kurtis Weissnat",
  "username": "Elwyn.Skiles",
  "email": "Telly.Hoeger@billy.biz",
  "address": {
    "street": "Rex Trail",
    "suite": "Suite 280",
    "city": "Howemouth",
    "zipcode": "58804-1099",
    "geo": {
      "lat": "24.8918",
      "lng": "21.8984"
    }
  },
  "phone": "210.067.6132",
  "website": "elvis.io",
  "company": {
    "name": "Johns Group",
    "catchPhrase": "Configurable multimedia task-force",
    "bs": "generate enterprise e-tailers"
  }
}
2.  Send a `PUT` request to the route `/posts` to change the title of the post with the `id` 57 to `"We The Best"`.
{
  "title": "We The Best",
  "id": 57
}

3.  Send a `DELETE` request to the route `/todos` to delete the Todo with the `id` 146.
{}
4.  Send a `POST` request to the route `/albums` to create an album with the `userId` 10 and the `title` "My Summer Vacation".
{
  "userId": "10",
  "title": "My Summer Vacation",
  "id": 101
}
5.  Send a `DELETE` request to the route `/users` to delete the user with the `id` 4.
{}
6.  Send a `PUT` request to the route `/todos` to change the `userId` of the Todo to 6 where the `id` of the Todo is 51.
{
  "userId": "6",
  "id": 51
}
7.  Send a `POST` request to the route `/photos` to add a picture of your choice with the `albumId` of 1.
{
  "title": "turtle",
  "url": "https://images2.minutemediacdn.com/image/upload/c_crop,h_2549,w_4536,x_0,y_237/f_auto,q_auto,w_1100/v1560186367/shape/mentalfloss/istock-687398754.jpg",
  "albumId": "1",
  "id": 5001
}
8.  Send a `GET` request to the route `/albums` to get the album with the `id` of 3.
{
  "userId": 1,
  "id": 3,
  "title": "omnis laborum odio"
}
9.  Send a `DELETE` request to the route `/posts` to delete the post with the `id` of 73.
{}
10. Send a `PUT` request to the route `/users` to create a user with the identity of your choice.
//can't create a new user with put.
