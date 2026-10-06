# GET /get dengan Query Params

**Tool:** Postman (Rizki Rofi's Workspace)

## Request
| Item | Nilai |
|------|-------|
| Method | `GET` |
| URL | `https://httpbin.org/get?nama=Rofi&kelas=TI` |
| Environment | No Environment |
| Headers | 7 |

### Query Params
| Key | Value |
|-----|-------|
| nama | Rofi |
| kelas | TI |

## Response
| Item | Nilai |
|------|-------|
| Status | **200 OK** |
| Waktu | 3.10 s |
| Ukuran | 687 B |
| Format Body | JSON |

### Body (sebagian yang terlihat)
```json
{
    "args": {
        "kelas": "TI",
        "nama": "Rofi"
    },
    "headers": {
        "Accept": "*/*",
        "Accept-Encoding": "gzip, deflate, br",
        "Cache-Control": "no-cache",
        "Host": "httpbin.org",
        "Postman-Token": "9d61cf5b-2a3c-4218-829a-564165d1e8e9",
        "User-Agent": "PostmanRuntime/2.10.1"
    }
}
```

## Keterangan
Parameter `nama` dan `kelas` dikirim lewat URL, lalu dikembalikan oleh server pada objek `args` di response.
