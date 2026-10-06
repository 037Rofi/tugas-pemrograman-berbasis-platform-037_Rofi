# Praktikum Postman – POST Data

**Nama:** Rofi
**NIM:** 2024520037
**Prodi:** Informatika

Collection: **My Collection** → request `Post data`

---

## Request

- Method: `POST`
- URL: `https://httpbin.org/post`
- Body: `raw` → `JSON`

```json
{
  "nama": "Rofi",
  "nim": "2024520037",
  "prodi": "Informatika"
}
```

---

## Response

- Status: `200 OK`
- Waktu: 23 ms
- Ukuran: 953 B

```json
{
    "args": {},
    "data": "{\r\n  \"nama\": \"Rofi\",\r\n  \"nim\": \"2024520037\",\r\n  \"prodi\": \"Informatika\"\r\n}",
    "files": {},
    "form": {},
    "headers": {
        "Accept": "*/*",
        "Accept-Encoding": "gzip, deflate, br",
        ...
    }
}
```

---

## Kesimpulan

Request **POST** mengirim data lewat *body* JSON. httpbin mengembalikannya pada field `data`, dan request berhasil dengan status `200 OK`.
