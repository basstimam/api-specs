# User Spec

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
  "message": "success!"
}
```

Response Body Error :
500

```json
{
  "errors": "internal server error"
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
    "message":"success",
}
```
Request Body Error :

500

```json
{
  "errors": "internal server error!"
}
```

## Delete User

Endpoint : Delete /user/:delete

Request Body Success :

```json
{
  "message": "user succesfuly fired!"
}
```
