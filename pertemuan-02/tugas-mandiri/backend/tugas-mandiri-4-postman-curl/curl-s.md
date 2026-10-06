# curl -s https://httpbin.org/get

**Tool:** Command Prompt (Windows, Version 10.0.28120.3122)

## Perintah
```
C:\Users\user>curl -s https://httpbin.org/get
```

## Output
```
{
  "args": {},
  "headers": {
    "Accept": "*/*",
    "Host": "httpbin.org",
    "User-Agent": "curl/8.21.0",
    "X-Amzn-Trace-Id": "Root=1-6ac4f88b-22d3cfb53c2b27546db40fa4"
  },
  "origin": "157.20.209.25",
  "url": "https://httpbin.org/get"
}
```

## Keterangan
Opsi `-s` (silent) menyembunyikan progress dan pesan error, serta **tidak menampilkan header response**. Yang tampil hanya body JSON, berbeda dengan `curl -i` yang juga menampilkan header.
