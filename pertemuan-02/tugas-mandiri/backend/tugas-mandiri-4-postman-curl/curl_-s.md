# curl -i https://httpbin.org/status/404

**Tool:** Command Prompt (Windows, Version 10.0.28120.3122)

## Perintah
```
C:\Users\user>curl -i https://httpbin.org/status/404
```

## Output
```
HTTP/1.1 404 NOT FOUND
Date: Tue, 06 Oct 2026 13:31:36 GMT
Content-Type: text/html; charset=utf-8
Content-Length: 0
Connection: keep-alive
Server: gunicorn/19.9.0
Access-Control-Allow-Origin: *
Access-Control-Allow-Credentials: true
```

## Keterangan
| Item | Nilai |
|------|-------|
| Status | **404 NOT FOUND** |
| Content-Length | 0 (body kosong) |
| Server | gunicorn/19.9.0 |

Opsi `-i` menampilkan header response bersama body. Body kosong karena endpoint `/status/404` hanya mensimulasikan status.
