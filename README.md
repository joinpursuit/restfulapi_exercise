# Interacting with APIs & Scavenger Hunt

In this exercises you will be retrieving information from an API as well as adding information for the API to save. By doing this exercises you will practice and reinforce.

* HTTP Methods
* The use of URL Query Parameters to filter results
* Making network requests with Postman or `curl`
* Learn about HTTP status codes

## Tasks

For this exercise use the Todos API.

* Docs: https://github.com/alejo4373/Todos-API
* Root Endpoint: https://alejos-todos-api.herokuapp.com

Try out all requests you can think of in this API, the docs are a good starting point.

In your fork of this repo create a `answers.json` file where you will put your answers. Copy the json bellow to your file.

1. For each request add a new object to the `requests` array in your json file, in the same format seen here.
2. Find all the 9 possible status codes this API returns and add them to `statusCodesFound` in your json file.

```json
{ 
  "requests": [
    {
      "method": <METHOD>,
      "endpoint": </api/something>,
      "description": <EXPLAIN WHAT THE REQUEST DID/DOES IN YOUR OWN WORDS>,
      "responseStatusCode": <###>,
      "statusCodeMeaning": <WHAT DOES THIS STATUS CODE MEAN>
    },
    {
      "method": "GET",
      "endpoint": "/api/todos",
      "description": "Returns a list of all todos",
      "responseStatusCode": 200,
      "statusCodeMeaning": "The request was successful"
    }
  ],
  "statusCodesFound": [200, ...]
}
```

### Scavenger Status Codes Hunt Hints

* It went just 🆗
* Users cannot have `fullname`
* There's one hint "hidden in plain sight" in the documentation of the API.
* Bad, bad, bad request!
* What does God got to do?
* Can't remove it twice?!?
* There's a lot of methods to try.
* How does this API handle duplicates?
* `200` is different from `201`?


<details>
<summary> Status Codes Scavenger Hunt answers </summary>

<details>
<summary> ⚠️ Are you sure? </summary>


| Status Code | Method             | Description                                                                                              |
| ----------- | ------------------ | -------------------------------------------------------------------------------------------------------- |
| `200`       | various            | When visiting the home page `/`, getting todos and users etc                                             |
| `201`       | `POST`             | When creating a todo or a user                                                                           |
| `400`       | `POST`             | When required fields are not passed in the body for creating a user or a todo                            |
| `401`       | any                | When trying to go to `/admin`                                                                            |
| `403`       | `GET`              | When trying to read God's todos                                                                          |
| `404`       | `GET|PATCH|DELETE` | When a todo is not found                                                                                 |
| `405`       | any                | When a method is not handled/allowed and is applied to an entire collection `/api/todos` or `/api/users` |
| `409`       | `POST`             | When signing a user that already exists (duplicate usernames)                                            |
| `500`       | `POST`             | When adding a user with more than one field in the body. e.g. with `username` and `fullname`             |

The easter egg endpoint has an easter egg status code

| Status Code | Method | Description                                  |
| ----------- | ------ | -------------------------------------------- |
| `418`       | `GET`  | At `/9` as the entry point to the easter egg |

</details>
</details>

### Bonuses

1. Take a look at the upcoming lessons to learn how to make make network requests with JavaScript.
Since you previously had build a simple Todos App with HTML and now you know how to manipulate
the DOM, add some JS to try to connect your Todos app to this API so that todos you enter in the page 
are saved to the API. Marking a todo as complete or uncompleted should work.
2. Find the easter egg hidden in the API.
