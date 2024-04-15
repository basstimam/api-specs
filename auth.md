# Auth Spec

## Login

Endpoint : GET /login

Request Body : 
```json
{
    "username" : "admin",
    "password" : "123",

}
```

Response Body Success : 
```json
{
   "data" : {
     "uuid":"fcb102903",
     "role":"dokter",
   },
   "message": "Login Berhasil!"

}
```

Response Body Error : 
404
```json
{
   "errors" : "account not found!"

}
```

400
```json
{
   "errors" : "wrong password!"

}
```

## Register User

Endpoint : POST /register-user

Request Body : 
```json
{
    "username" : "admin",
    "password" : "123",
    "full_name" : "Dr imam SPDI",
    "role" : "Doctor"
}
```

Ressponse Body Success : 
```json
{
   "message": "user register as ${role}!"
}
```
Response Body Error : 

400
```json
{
   "errors" : "field username is required!"

}
```

## Change Password

Endpoint : POST /change-pw/userid

Request Body : 
```json
{
    "new_password" : "123",
    "confirm_password" : "123",
}
```

Response Body Success : 
```json
{
   "message": "password succesfuly change!"
}
```
Response Body Error : 

400
```json
{
   "errors" : "passwordn not same!"

}
```


