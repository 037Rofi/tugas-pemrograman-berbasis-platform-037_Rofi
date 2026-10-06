# curl -i https://httpbin.org/get

**Tool:** Command Prompt (Windows, Version 10.0.28120.3122)

## Perintah
```
C:\Users\user>curl -i https://httpbin.org/get
```

## Output
```
HTTP/1.1 200 OK
Date: Tue, 06 Oct 2026 13:30:31 GMT
Content-Type: application/json
Content-Length: 255
Connection: keep-alive
Server: gunicorn/19.9.0
Access-Control-Allow-Origin: *
Access-Control-Allow-Credentials: true

{
  "args": {},
  "headers": {
    "Accept": "*/*",
    "Host": "httpbin.org",
    "User-Agent": "curl/8.21.0",
    "X-Amzn-Trace-Id": "Root=1-6ac4f7f7-2da74333417a65850d680d7e"
  },
  "origin": "157.20.209.25",
  "url": "https://httpbin.org/get"
}
```

## Keterangan
| Item | Nilai |
|------|-------|
| Status | **200 OK** |
| Content-Type | application/json |
| Content-Length | 255 |
| User-Agent | curl/8.21.0 |

Response berisi `args` kosong (tidak ada query param), header yang dikirim curl, IP asal (`origin`), dan URL request.
