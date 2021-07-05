Tasks 

###Users
1.  Request: GET  '/users'

    Response:
    ```json
    {
        "id": 1,
        "username": "alejo4373"
        },
    ```
    This retrieves a list of all the users; id and username
-------------------------------------------------------------
    Request: GET '/users/3Chainz'
    Response:
    ```json
    {
    "payload": {
        "id": 4,
        "username": "3Chainz"
    },
    "err": false
}

    This retrieves a specific user; 3Chainz

-------------------------------------------------------------
    Request: POST '/users/signup'
    Body:
    ```json
    {
        "username": "Jonezy"
    }

    Response:
    {
    "payload": {
        "user": {
            "id": 47,
            "username": "Jonezy"
        },
        "msg": "User created"
    },
    "err": false
}

    This creates a new user called 'Jonezy' and assigns a new id ('47') to it

-------------------------------------------------------------

###Todos

    Request: GET  '/todos'
    Response:
    ```json
    {
            "id": "ecf57050",
            "owner": "AnimalCrackerEater",
            "text": "Leave Crackers on the sofa",
            "completed": false
        },
    ```

    This retrieves a list of all the todos objects; id, owner, the todo, and whether its completed or not 
-------------------------------------------------------------
    Request: POST '/todos'
    Body:
    ```json
    {
        owner: 'Jonezy'
        text: 'Read a book'
    }

    Response: 
    {
    "payload": {
        "id": "0c5c8720",
        "owner": "Jonezy",
        "text": "Read a book",
        "completed": false
    },
    "err": false
}
```
-------------------------------------------------------------
    This creates a new todo(Read a book) with a new owner(Jonezy)

    Request: GET '/todos/0c5c8720'

    Response:
     {
    "payload": {
        "id": "0c5c8720",
        "owner": "Jonezy",
        "text": "Read a book",
        "completed": false
    },
    "err": false
}

    This retrieves the new todo by its unique id
-------------------------------------------------------------
    Request: PUT  '/todos/0c5c8720'

    Body:
    {
        owner:Jonezy
        text:Read a book
        completed:true
    }

    Response:
    {
    "payload": {
        "id": "0c5c8720",
        "owner": "Jonezy",
        "text": "Read a book",
        "completed": true
    },
    "err": false
}

    Changes completed from false to true 
-------------------------------------------------------------
    Request: PATCH  '/todos/0c5c8720'

    Body:
    {
        owner:Jonezy
        text:Eat dinner
        completed: true
    }

    Response:
    {
    "payload": {
        "id": "0c5c8720",
        "owner": "Jonezy",
        "text": "Eat dinner",
        "completed": true
    },
    "err": false
}
    Changes text to 'Eat dinner'
-------------------------------------------------------------

    Request: DELETE '/todos/0c5c8720'

    Response:
    {
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}

    Deletes the whole todo object
-------------------------------------------------------------

2. 405
   404
   400
   409
   200
   201

