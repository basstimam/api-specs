# Poli Spec

## Create Poli

Endpoint : Post api/poli

Request body :

```json
{
  "name": "umum"
}
```

Response Body Success :

```json
{
  "status_code": 200,
  "message": "berhasil menambah poli"
}
```

## Add member Poli

Endpoint : Post api/poli/add-member
//post nya ke t poli
Request body :

```json
{
  "poli_id": 1,
  "user_id": 1
}
```

Response Body Success :

```json
{
  "status_code": 200,
  "message": "berhasil menambah member"
}
```

## Get All Poli User

Endpoint : GET /poli?page=1

Response Body Success :

```json
{
  "data": [
    {
      "id": "fcb102903",
      "poli_name": "azki"
    },
    {
      "id": "fcb102903",
      "poli_name": "azki"
    },
    {
      "id": "fcb102903",
      "poli_name": "azki"
    }
  ],
  "page": "1",
  "size": "3",
  "total_page": "20",
  "total_data": "60",
  "message": "success!",
  "status_code": 200
}
```

Response Body Error :
500

```json
{
  "status_code": 500,
  "message": "internal server error"
}
```

## Detail Poli

Endpoint : GET /poli/:poliId
Response Body Success :

```json
{
  "data": [
    {
      "id": "fcb102903",
      "name": "umum",
      "doctor":"azki"
    },
    {
      "id": "fcb102903",
      "name": "anak",
      "doctor":"azki"
    },
    {
      "id": "fcb102903",
      "name": "gigi",
      "doctor":"azki"
    }
  ],
  "page": "1",
  "size": "3",
  "total_page": "20",
  "total_data": "60",
  "message": "success!",
  "status_code": 200
}
```

Request Body Error :

500

```json
{
  "status_code": 500,
  "message": "internal server error!"
}
```