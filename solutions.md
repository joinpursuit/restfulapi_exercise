# Todos API

### Root https://fsw62-todos-api.herokuapp.com/api

### Resources
* users
* todos

### Endpoints

#### Users
| Method | Endpoint           | What does this do? |
|--------|--------------------|--------------------|
| `GET`  | `/users`           | `This returns 5 users listing both their ID# and their User Name. It also informs the requester that there were no errors in their request.`|
| `GET`  | `/users/<user-id>` | `It returns an alert letting the requester know that there are no instaces of what they were looking for at that endpoint because there are no parameters with the title "user-id". It also returns a notification for the requester to let them know there were no errors made in their request attempt`|
| `POST`  | `/users/signup`   | `Posting to this endpoint without parameters declaring the user name and id # of a new user brings an error message explaining that the requester needs to include these parameters to be able to post in this fashion.`|


* Fill in the blanks above :arrow_up: 

#### Todos
| Method   | Endpoint           | What does this do? | Possible Query Params |
|----------|--------------------|--------------------|-----------------------|
| `GET`    | `/todos`           | `This returns a list of six todo items by three authors, including their ID, the user name of the owner under "owner", the text of their todo item, and a qualifier letting the requester see if the todo item has been completed or not.`| `username=<username>`, `completed=<true|false> `
| `POST`   | `/todos`           | `This allows requesters to post items to the todo list. However, you need to specify the parameters "owner" (existing users only) and "text" (the note attached with the reminder for the user's todo list library)`||
| `GET`    | `/todos/<todo-id>` | `This allows the requester (with the specific server generated todo-id to read the entierety of the information housed in the todo item at that specific id`||
| `PUT`    | `/todos/<todo-id>` | `This allows the requester to change the entirety of thie todo item housed at the specific todo-id. This change is permanant, and if it is missing any information - it will omit that information in the update.`||
| `PATCH`  | `/todos/<todo-id>` | `This allows a requester to change the data housed in only one parameter without altering or removing any of the other data housed at that todo-id.`||
| `DELETE` | `/todos/<todo-id>` | `This removes the todo item at this todo-id completely. It can not be recovered.`||

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