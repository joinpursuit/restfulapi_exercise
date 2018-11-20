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
    "userId ": "10",
    "title": "My Summer Vacation",
    "id": 101
}

5.  Send a `DELETE` request to the route `/users` to delete the user with the `id` 4.

{}

6.  Send a `PUT` request to the route `/todos` to change the `userId` of the Todo to 6 where the `id` of the Todo is 51.

{
    "userId ": "6",
    "id": 51
}

7.  Send a `POST` request to the route `/photos` to add a picture of your choice with the `albumId` of 1.

{
    "albumId": "1",
    "title": "dlkafjldaskjfasdljflsa",
    "url": "https://vignette.wikia.nocookie.net/dragonballfanon/images/7/70/Random.png/revision/latest?cb=20161221030547",
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
    "id": "1123",
    "name": "Treagan Birbal",
    "username": "treagan.birbal",
    "email": "treagan.birbal@email.com",
    "phone": "387923873"
}
