<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->

- [Response API](#response-api)
    - [Contoh Response Umumnya](#contoh-response-umumnya)
    - [Response dengan Pagination](#response-dengan-pagination)
    - [Contoh Response Error](#contoh-response-error)
    - [Response Error Pada Kolom Tertentu](#response-error-pada-kolom-tertentu)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->


# Response API

Dalam penentuan response api tidak ada standarisasinya, tetapi kita harus membuat dengan konsisten dan informasi jelas dibutuhkan.
Selain itu untuk patter yang sering digunakan adalah code, status, dan data. Status code yang sering digunakan yaitu sebagai berikut:

- 1xx (Informasi Response) <!-- Jarang Digunakan -->
- 2xx (Success Response) 
- 3xx (Redirect Response) <!-- Jarang Digunakan-->
- 4xx (Client Error Response)
- 5xx (Server Error Response)

Lengkap https status code di website [mdn docs]

[mdn docs]: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status#informational_responses

### Contoh Response Umumnya

```json
{
  "code": 200, // opsional
  "status": "success", // opsional
  "data": [
    {"id": 1, "name": "asraf", dll},
    {"id": 2, "name": "takayums", dll},
    {"id": 3, "name": "yuma", dll}]
}
```

### Response dengan Pagination

```json
{
  "code": 200, // opsional
  "status": "success", // opsional
  "data": [
    {"id": 1, "name": "asraf", dll},
    {"id": 2, "name": "takayums", dll},
    {"id": 3, "name": "yuma", dll}
  ],
  "page": {
    "size": 10,
    "total": 100,
    "totalPage": 10,
    "current": 1,
  }
}
```

### Contoh Response Error

```json
{
  "code": 500,
  "status": "Server Down",
  "error": [
    "Some error", "Error 1", "Error 2", dst
  ]
}
```

### Response Error Pada Kolom Tertentu 

```json
{
  "code": 500,
  "status": "Server Down",
  "error": {
    "id": [
      "must be not null",
      "must be number"
    ],
    "name": [
      "must be not null",
      "must be string"
    ]
  }
}
```
