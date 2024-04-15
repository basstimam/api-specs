# Profile Spec

## Login

Endpoint : GET /users?page=1

Response Body Success : 
```json
{
   "data" : [
        {
            "uuid":"fcb102903",
            "username":"azki",
            "fullname":"azkia ajmal fairuz",
            "role":"dokter",
        },
        {
            "uuid":"fcb102903",
            "username":"azki",
            "fullname":"azkia ajmal fairuz",
            "role":"dokter",
        },
        {
            "uuid":"fcb102903",
            "username":"azki",
            "fullname":"azkia ajmal fairuz",
            "role":"dokter",
        },
   ],
   "page":"1",
   "size":"3",
   "total_page":"20",
   "total_data":"60",
   "message": "success!"

}
```

Response Body Error : 
500
```json
{
   "errors" : "internal server error"

}
```

## Register User

Endpoint : GET /register-user

Request Body : 
```json
{
    "username" : "admin",
    "password" : "123",
    "full_name" : "Dr imam SPDI",
    "role" : "Doctor"
}
```

Request Body Success : 
```json
{
   "message": "user register as ${role}!"
}
```
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

Request Body Success : 
```json
{
   "message": "password succesfuly change!"
}
```
400
```json
{
   "errors" : "passwordn not same!"

}
```


