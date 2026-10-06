# GET /get

**Tool:** Postman (Rizki Rofi's Workspace)

## Request
| Item | Nilai |
|------|-------|
| Method | `GET` |
| URL | `https://httpbin.org/get` |
| Environment | No Environment |
| Query Params | Kosong |
| Headers | 7 |

## Response
| Item | Nilai |
|------|-------|
| Status | **200 OK** |
| Waktu | 1.50 s |
| Ukuran | 626 B |
| Format Body | JSON |

### Body (sebagian yang terlihat)
```json
{
    "args": {},
    "headers": {
        "Accept": "*/*",
        "Accept-Encoding": "gzip, deflate, br",
        "Cache-Control": "no-cache",
        "Host": "httpbin.org",
        "Postman-Token": "235dc08e-9cd9-4e9c-9432-a15a1b24c393",
        "User-Agent": "PostmanRuntime/2.10.1",
        "X-Amzn-Trace-Id": "Root=1-6ac4f6b9-43b244881285423b3f992cb4"
    },
    "origin": "157.20.209.25",
    ...
```

## Keterangan
Request GET tanpa parameter sehingga `args` kosong. Response menampilkan header yang dikirim Postman dan IP asal (`origin`).
