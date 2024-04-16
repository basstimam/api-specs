# Doctor API SPEC

## Periksa Pasien

Endpoint : Post periksa
Request Body :

```json
{
  "pasien_id": 1,
  "status": "PEMERIKSAAN"
}
```
Response Body Success :

```json
{
  "status_code": 200,
  "message": "status pasien berubah"
}
```

## Diagnosa Passien

Endpoint : Post diagnosa
Request Body :
//post ke table resep dan pengambilan obat
```json
{
  "pasien_id": 1,
  "keterangan": "blblblbl",
  "hasil_diagnosa": "autis",
  "user_id":"fcaskjijw",
  "status": "SELESAI"
}
```

Response Body Success :

```json
{
  "status_code": 200,
  "message": "berhasil mendiagnosa user"
}
```
