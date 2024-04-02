# Client API SPEC

## Register BPJS

Endpoint : POST /register

Request Body : 
```json
{
    "nomor_bpjs" : "123123123",
    "nama" : "Imam",
    "nik"  : "123123123"
}
```

Response Body Success : 

```json
{
    "message" : "Anda antrian ke ${queue}"
    
}
```

Response Body Error : 

```json
{
    "errors" : "Bad Request"
}
```