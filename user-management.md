# User Spec


## Create User
Endpoint : Post user

Request body :

```json
    {
      "username": "azki",
      "fullname": "azkia ajmal fairuz",
      "password":"isvillc15001",
      "role": "dokter",
    }
```

Response Body Success :

```json
{
  "status_code": 200,
  "message": "berhasil menambah user"
}
```
## Get List User

Endpoint : GET /users?page=1

Response Body Success :

```json
{
  "data": [
    {
      "uuid": "fcb102903",
      "username": "azki",
      "fullname": "azkia ajmal fairuz",
      "role": "dokter"
    },
    {
      "uuid": "fcb102903",
      "username": "azki",
      "fullname": "azkia ajmal fairuz",
      "role": "dokter"
    },
    {
      "uuid": "fcb102903",
      "username": "azki",
      "fullname": "azkia ajmal fairuz",
      "role": "dokter"
    }
  ],
  "page": "1",
  "size": "3",
  "total_page": "20",
  "total_data": "60",
  "message": "success!",
  "status_code":200,

}
```

Response Body Error :
500

```json
{
  "status_code":500,
  "message": "internal server error"
}
```

## Detail User

Endpoint : GET /user/:userId
Response Body Success :

```json
{
    "data":{
        "uuid":"fcb102903",
        "username":"azki",
        "fullname":"azkia ajmal fairuz",
        "role":"dokter",
    },
    "status_code":200,
    "message":"success",
}
```
Request Body Error :

500

```json
{
  "status_code":500,
  "message": "internal server error!"
}
```

## Delete User

Endpoint : Delete /user/:delete

Request Body Success :

```json
{
  "status_code":200,
  "message": "user succesfuly fired!"
}
```
