# Antrian Spec


## get antrian for docter
Endpoint : Get antrian/:doctor?page=1

Request params :

```json
    {
      "id_dokter": "asdasdfadsf",
      "page":1
    }
```
Response Body Success :

```json
{
  "data": [
    {
      "nomor_bpjs": "309293099",
      "nama_passien": "azkia ajmal fairuz",
      "dokter": "iimama",
      "poli":"umum",
      "status": "menunggu"
    },
    {
      "nomor_bpjs": "309293099",
      "nama_passien": "azkia ajmal fairuz",
      "dokter": "iimama",
      "poli":"umum",
      "status": "menunggu"
    },
    {
      "nomor_bpjs": "309293099",
      "nama_passien": "azkia ajmal fairuz",
      "dokter": "iimama",
      "poli":"umum",
      "status": "menunggu"
    },
   
  ],
  "page": "1",
  "size": "3",
  "total_page": "20",
  "total_data": "60",
  "message": "success!",
  "status_code":200,

}
```

## get antrian for apoteker
Endpoint : Get antrian?page=1

Request params :

```json
    {
      "page":1
    }
```
Response Body Success :

```json
{
  "data": [
    {
      "nomor_bpjs": "309293099",
      "nama_passien": "azkia ajmal fairuz",
      "hasil_diagnosa": "azkia ajmal fairuz",
      "keterangan_resep": "azkia ajmal fairuz",
      "dokter": "iimama",
      "poli":"umum",
      "status": "PICKUP"
    },
    {
      "nomor_bpjs": "309293099",
      "nama_passien": "azkia ajmal fairuz",
      "hasil_diagnosa": "azkia ajmal fairuz",
      "keterangan_resep": "azkia ajmal fairuz",
      "dokter": "iimama",
      "poli":"umum",
      "status": "PICKUP"
    },
    {
      "nomor_bpjs": "309293099",
      "nama_passien": "azkia ajmal fairuz",
      "hasil_diagnosa": "azkia ajmal fairuz",
      "keterangan_resep": "azkia ajmal fairuz",
      "dokter": "iimama",
      "poli":"umum",
      "status": "PICKUP"
    },
  ],
  "page": "1",
  "size": "3",
  "total_page": "20",
  "total_data": "60",
  "message": "success!",
  "status_code":200,

}
```