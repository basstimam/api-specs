# Doctor API SPEC

# Passien API SPEC



## Get List Passien by poli 

Endpoint : GET doctor/?page=1

Response Body Success : 
```json
{
  "data": [
    {
      "passien_id": "1",
      "nomor_bpjs": "309293099",
      "nama_passien": "azkia ajmal fairuz",
      "tanggal_lahir": "04-12-2023",
      "alamat":"palasari",
      "faskes_tingkat_satu":"puskesmas",
      "poli":"umum"
    },
    {
      "passien_id": "1",
      "nomor_bpjs": "309293099",
      "nama_passien": "azkia ajmal fairuz",
      "tanggal_lahir": "04-12-2023",
      "alamat":"palasari",
      "faskes_tingkat_satu":"puskesmas",
      "poli":"umum"
    },
    {
      "passien_id": "1",
      "nomor_bpjs": "309293099",
      "nama_passien": "azkia ajmal fairuz",
      "tanggal_lahir": "04-12-2023",
      "alamat":"palasari",
      "faskes_tingkat_satu":"puskesmas",
      "poli":"umum"
    },
  ],
  "page": "1",
  "size": "3",
  "total_page": "20",
  "total_data": "60",
  "message": "success!",
  "status_code": 200
}
```