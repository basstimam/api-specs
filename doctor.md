# Doctor API SPEC

## Diagnosa Passien

Endpoint : Post diagnosa/:pasienId
Request Body :

```json
{
  "keterangan": "blblblbl",
  "hasil_diagnosa": "autis",
  "status":"SELESAI"
}
```

Response Body Success :

```json
{
  "status_code": 200,
  "message": "berhasil mendiagnosa user"
}
```
