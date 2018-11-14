# RESTful API Practice

Create a README (`.md`) file and paste all of the responses from the server for each request. Utilize the [JSON Placeholder API](https://jsonplaceholder.typicode.com/) for each request.

1.  Send a `GET` request to the route `/users` to get the user with the `id` 7.
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
2.  Send a `PUT` request to the route `/posts` to change the title of the post with the `id` 57 to `"We The Best"`.
    {
    "userId": 6,
    "id": 57,
    "title": "We The Best",
    "body": "at pariatur consequuntur earum quidem\nquo est laudantium soluta voluptatem\nqui ullam et est\net cum voluptas voluptatum repellat est"
    }
3.  Send a `DELETE` request to the route `/todos` to delete the Todo with the `id` 146.
    {}
4.  Send a `POST` request to the route `/albums` to create an album with the `userId` 10 and the `title` "My Summer Vacation".
    "userId": "10",
    "title": "My summer Vacation",
    "id": 101
    }

5.  Send a `DELETE` request to the route `/users` to delete the user with the `id` 4.
    {}
6.  Send a `PUT` request to the route `/todos` to change the `userId` of the Todo to 6 where the `id` of the Todo is 51.

{
"userId": "6",
"id": 51
}

7.  Send a `POST` request to the route `/pictures` to add a picture of your choice with the `albumId` of 1.

{
"albumId": "1",
"url": "https://i.ytimg.com/vi/Yj7ja6BANLM/maxresdefault.jpg",
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

{
"id": 5,
"name": "jon",
"email": "asf@gmail.com"
}
