# Praktikum Postman – GET Data

**Nama:** Rofi
**NIM:** 2024520037
**Prodi:** Informatika

Collection: **My Collection** → request `Get data`

---

## Request

- Method: `GET`
- URL: `https://httpbin.org/get?Nama=Rofi&Nim=2024520037`

**Query Params**

| Key  | Value      |
|------|------------|
| Nama | Rofi       |
| Nim  | 2024520037 |

---

## Response

- Status: `200 OK`
- Waktu: 23 ms
- Ukuran: 724 B

```json
{
    "args": {
        "Nama": "Rofi",
        "Nim": "2024520037"
    },
    "headers": {
        "Accept": "*/*",
        "Accept-Encoding": "gzip, deflate, br",
        "Cache-Control": "no-cache",
        ...
    }
}
```

---

## Kesimpulan

Request **GET** mengirim data lewat *query parameter* di URL. httpbin mengembalikannya pada field `args`, dan request berhasil dengan status `200 OK`.
