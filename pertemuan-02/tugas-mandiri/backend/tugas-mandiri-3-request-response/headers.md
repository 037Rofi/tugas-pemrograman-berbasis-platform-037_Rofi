# GET /headers

**Tool:** Postman (Rizki Rofi's Workspace)

## Request
| Item | Nilai |
|------|-------|
| Method | `GET` |
| URL | `https://httpbin.org/headers` |
| Environment | No Environment |
| Query Params | Kosong |
| Headers | 7 |

## Response
| Item | Nilai |
|------|-------|
| Status | **200 OK** |
| Waktu | 1.03 s |
| Ukuran | 544 B |
| Format Body | JSON |

### Body
```json
{
    "headers": {
        "Accept": "*/*",
        "Accept-Encoding": "gzip, deflate, br",
        "Cache-Control": "no-cache",
        "Host": "httpbin.org",
        "Postman-Token": "a75fa690-6908-4821-a083-04ad5cea8ef6",
        "User-Agent": "PostmanRuntime/2.10.1",
        "X-Amzn-Trace-Id": "Root=1-6ac4f492-5657c77a5cf737873f37aa00"
    }
}
```

## Keterangan
Endpoint `/headers` mengembalikan header HTTP yang dikirim oleh client, sehingga berguna untuk melihat header apa saja yang ikut terkirim oleh Postman.
