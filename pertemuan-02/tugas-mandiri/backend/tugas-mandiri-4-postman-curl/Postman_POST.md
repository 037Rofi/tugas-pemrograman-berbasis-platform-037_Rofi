# POST /post

**Tool:** Postman (Rizki Rofi's Workspace)

## Request
| Item | Nilai |
|------|-------|
| Method | `POST` |
| URL | `https://httpbin.org/post` |
| Environment | No Environment |
| Headers | 9 |
| Body Type | raw (JSON) |

### Body Request
```json
{
  "nama": "Rofi",
  "kelas": "Informatika"
}
```

## Response
| Item | Nilai |
|------|-------|
| Status | **200 OK** |
| Waktu | 1.62 s |
| Ukuran | 872 B |
| Format Body | JSON |

### Body (sebagian yang terlihat)
```json
{
    "args": {},
    "data": "{\r\n  \"nama\": \"Rofi\",\r\n  \"kelas\": \"Informatika\"\r\n}",
    "files": {},
    "form": {},
    "headers": {
        "Accept": "*/*",
        "Accept-Encoding": "gzip, deflate, br",
        "Cache-Control": "no-cache",
        "Content-Length": "49",
        "Content-Type": "application/json",
        "Host": "httpbin.org",
        ...
```

## Keterangan
Data JSON yang dikirim muncul di field `data` pada response. Field `form` kosong karena data dikirim sebagai raw JSON, bukan form.
