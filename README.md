# try_curl

## ダウンロードのトレースを出力する

```
$ curl [URL] --trace-time --trace-ascii -
07:54:28.349906 == Info: Host repo1.maven.org:443 was resolved.
07:54:28.349961 == Info: IPv6: 2a04:4e42:2e::209
07:54:28.349964 == Info: IPv4: 151.101.196.209
07:54:28.349993 == Info:   Trying 151.101.196.209:443...
07:54:28.365925 == Info: Connected to repo1.maven.org (151.101.196.209) port 443
07:54:28.367140 == Info: ALPN: curl offers h2,http/1.1
07:54:28.367279 => Send SSL data, 5 bytes (0x5)

...

07:54:28.721225 == Info: SSL connection using TLSv1.2 / ECDHE-RSA-CHACHA20-POLY1305 / X25519 / RSASSA-PSS
07:54:28.721245 == Info: ALPN: server accepted h2
07:54:28.721276 == Info: Server certificate:
07:54:28.721317 == Info:  subject: CN=repo1.maven.org
07:54:28.721350 == Info:  start date: Oct 19 15:00:14 2024 GMT
07:54:28.721365 == Info:  expire date: Nov 20 15:00:13 2025 GMT
07:54:28.721420 == Info:  subjectAltName: host "repo1.maven.org" matched cert's "repo1.maven.org"
07:54:28.721456 == Info:  issuer: C=BE; O=GlobalSign nv-sa; CN=GlobalSign Atlas R3 DV TLS CA 2024 Q4
07:54:28.721473 == Info:  SSL certificate verify ok.

...

07:54:29.052495 == Info: Connection #0 to host repo1.maven.org left intact
```
