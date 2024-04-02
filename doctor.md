# User API SPEC



## Login User API

Endpoint : POST users/login

Request Body : 
```json
{
    "username" : "apoteker",
    "password" : "123",

}
```

Request Body Success : 
```json
{
   "data" : {
     "token" : "unique-token"
   }

}
```

Response Body Error : 

```json
{
   "errors" : "Username or password wrong!"

}
```










