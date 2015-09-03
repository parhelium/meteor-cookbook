## How can I see what ports are open on my machine?

```
$ sudo netstat -tulpn | grep LISTEN
tcp        0      0 127.0.0.1:53            0.0.0.0:*               LISTEN      5452/dnsmasq
tcp        0      0 127.0.0.1:631           0.0.0.0:*               LISTEN      1037/cupsd
tcp6       0      0 ::1:631                 :::*                    LISTEN
```