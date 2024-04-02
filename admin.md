# Admin API Spec

## Login

Endpoint : POST /login-as-admin

Request Body : 
```json
{
    "username" : "admin",
    "password" : "123",

}
```

Request Body Success : 
```json
{
   "data" : {
     "token" : "unique-token",
     "role":{
        "role_id": "0",
        "role":"admin",
     },
     "message": "Login Berhasil!"
   }

}
```

Response Body Error : 

```json
{
   "errors" : "Username or password wrong!"

}
```

## Get All Users

Endpoint : GET /admin/get-all-user

Header : 
- Authorization : token


```json
{
   "data" : [
    {
        "id": 1,
        "first_name": "Imam",
        "last_name": "Fahrudin",
        "username": "imam-doctor",
        "role":{
        "role_id": "1",
        "role":"doctor",
     }
    },
     {
        "id": 2,
        "first_name": "Heidi",
        "last_name": "",
        "username": "heidi-apoteker",
        "role":{
        "role_id": "2",
        "role":"apoteker",
     },
   ]

}
```

Response Body Error : 

```json
{
    "errors" :  "Unathorized!"
}
```


## Edit User API
Endpoint : PATCH /admin/edit-user/:id

Headers : 
- Authorization : token

Request Body :

```json
{
   "data" : 
    {
        ,
        "first_name": "Imam", //optional
        "last_name": "Fahrudin",//optional
        "username": "imam-doctor",//optional
        "role":{
        "role_id": "1",//optional
        "role":"doctor",//optional
     }
    },
   

}
```

## Remove User API

Endpoint : DELETE /admin/delete-user/id

Headers : Authorization : token

Response Body Success : 

```json
{
    "data" :  "OK"
}
```

Response Body Error : 

```json
{
    "errors" :  "User not found!"
}
```




