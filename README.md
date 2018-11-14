1.  Send a `GET` request to the route `/users` to get the user with the `id` 7.

https://jsonplaceholder.typicode.com/users/7
```js
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
```

2.  Send a `PUT` request to the route `/posts` to change the title of the post with the `id` 57 to `"We The Best"`.
https://jsonplaceholder.typicode.com/posts/57
I used `PATCH` instead.

```js
{
    "userId": 6,
    "id": 57,
    "title": "We The Best",
    "body": "at pariatur consequuntur earum quidem\nquo est laudantium soluta voluptatem\nqui ullam et est\net cum voluptas voluptatum repellat est"
}

```


3.  Send a `DELETE` request to the route `/todos` to delete the Todo with the `id` 146.
https://jsonplaceholder.typicode.com/todos/146

```js

{}

```


4.  Send a `POST` request to the route `/albums` to create an album with the `userId` 10 and the `title` "My Summer Vacation".

```js



```


5.  Send a `DELETE` request to the route `/users` to delete the user with the `id` 4.

```js



```


6.  Send a `PUT` request to the route `/todos` to change the `userId` of the Todo to 6 where the `id` of the Todo is 51.

```js



```


7.  Send a `POST` request to the route `/pictures` to add a picture of your choice with the `albumId` of 1.

```js



```


8.  Send a `GET` request to the route `/albums` to get the album with the `id` of 3.

```js



```


9.  Send a `DELETE` request to the route `/posts` to delete the post with the `id` of 73.

```js



```


10. Send a `PUT` request to the route `/users` to create a user with the identity of your choice.

```js



```
