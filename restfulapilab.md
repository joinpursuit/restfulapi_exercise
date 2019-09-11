"PART 1"
1. **Request**: https://fsw62-todos-api.herokuapp.com/api/users
**Body**: N/A
**Response**:{
    "payload": [
        {
            "id": 1,
            "username": "alejo4373"
        },
        {
            "id": 2,
            "username": "JRJRocks"
        },
        {
            "id": 3,
            "username": "Mike923"
        },
        {
            "id": 4,
            "username": "3Chainz"
        },
        {
            "id": 5,
            "username": "George W. Swoosh"
        },
        {
            "id": 6,
            "username": "A pimp named slickback"
        },
        {
            "id": 7,
            "username": "okurrrt"
        }
    ],
    "err": false
}
**What does it do?**: obtains all users id # and usernames

2. **Request**: https://fsw62-todos-api.herokuapp.com/api/users/alejo4373
**Body**: N/A
**Response**: {
    "payload": {
        "id": 1,
        "username": "alejo4373"
    },
    "err": false
}
**What does it do?**: obtains specific user but only with username, not with id #


3. **Request**: https://fsw62-todos-api.herokuapp.com/api/users/signup
**Body**: id: 13
username: theRealObama
**Response**:
        {
            "id": 12,
            "username": " theRealObama"
        },
**What does it do?**: creates a new user and arranges their id # in the next order

4. **Request**: https://fsw62-todos-api.herokuapp.com/api/todos
**Body**: N/A
**Response**: {
    "payload": [
        {
            "id": "ecf57050",
            "owner": "AnimalCrackerEater",
            "text": "Leave Crackers on the sofa",
            "completed": false
        }, 
        etc....
**What does it do?**: obtains all todos in the entire list

5. **Request**: https://fsw62-todos-api.herokuapp.com/api/todos
**Body**:
    id: 1350
    owner: theRealObama
    text: make pancakes
**Response**:{
    "payload": {
        "id": " 1350",
        "owner": " theRealObama",
        "text": " make pancakes",
        "completed": false
    },
    "err": false
}
**What does it do?**: posts a new todo in whole list under specified id #, username and task

6. **Request**: https://fsw62-todos-api.herokuapp.com/api/todos/ 1350
**Body**: N/A
**Response**:         {
            "id": " 1350",
            "owner": " theRealObama",
            "text": " Make pancakes",
            "completed": false
        },
**What does it do?**: using the id # of the post you can retieve a specific one

7. **Request**: https://fsw62-todos-api.herokuapp.com/api/todos/ 1350?id= 1350&owner= theRealObama&text=take toilet paper
**Body**:id: 1350
owner: theRealObama
text:take toilet paper
completed:true
**Response**:          {
            "id": " 1350",
            "owner": " theRealObama",
            "text": " take toilet paper",
            "completed": "true"
        },
**What does it do?**: using the parameters of id, username and text you can replace a task

8. **Request**: https://fsw62-todos-api.herokuapp.com/api/todos/ 1350
**Body**: id: 1350
owner: theRealObama
text:take toilet paper
completed:false
**Response**:          {
            "id": " 1350",
            "owner": " theRealObama",
            "text": " take toilet paper",
            "completed": "false"
        },
**What does it do?**: makes minor changes within an existing post (in here it was the true/false)

9. **Request**: https://fsw62-todos-api.herokuapp.com/api/todos/ 1350
**Body**: id: 1350
owner: theRealObama
text:take toilet paper
completed:false
**Response**: N/A
**What does it do?**: deletes a post based on specified id #

"PART 2"
1. **Request**: https://fsw62-todos-api.herokuapp.com/api/todos/ 1350 // (once post was deleted)
**Status Code**: 404 NOT FOUND
**Response**: {
    "payload": {
        "msg": "Todo not found"
    },
    "err": true
}

2. **Request**: https://fsw62-todos-api.herokuapp.com/api/users 
**Status Code**: 200 OK
**Response**:     "payload": [
        {
            "id": 1,
            "username": "alejo4373"
        },
3. **Request**: https://fsw62-todos-api.herokuapp.com/api/users/signup?"id"= "5";&"username"= "gisellesanchez"
**Status Code**: 400 BAD REQUEST
**Response**: {
    "payload": "Expected valid values for user [username]",
    "err": true
}
4. **Request**:
**Status Code**: nah nah nah
**Response**:
