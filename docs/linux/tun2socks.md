---
hide:
 - toc
 - path
 - title
---

Linux Tun2Socks [Github](https://github.com/iamtrazy/xray-tun2socks)

---
Linux Proxy 

```
/etc/environment

export socks_proxy="socks://127.0.0.1:10808/"
export all_proxy="socks://127.0.0.1:10808/"
export no_proxy="localhost,127.0.0.0/8,::1"

export SOCKS_PROXY="socks://127.0.0.1:10808/"
export ALL_PROXY="socks://127.0.0.1:10808/"
export NO_PROXY="localhost,127.0.0.0/8,::1"



to check current proxy settings - env | grep proxy

```
---
Example XRay Config
```
{
  "inbounds": [
    {
      "port": 10808,
      "protocol": "socks",
      "listen": "127.0.0.1",
      "settings": {
        "auth": "noauth",
        "udp": true
      }
    }
  ],
  "outbounds": [
    {
      "protocol": "vmess",
      "settings": {
        "vnext": [
          {
            "address": "103.253.26.220",
            "port": 443,
            "users": [
              {
                "id": "42d6c190-ae7d-11ed-b134-205c6d5f5d78",
                "alterId": 0,
                "encryption": "none",
                "flow": ""
              }
            ]
          }
        ],
        "port": 0,
        "packetEncoding": "xudp",
        "mtu": 0
      },
      "streamSettings": {
        "network": "ws",
        "security": "tls",
        "tlsSettings": {
          "allowInsecure": true,
          "serverName": "ar.linkedin.com"
        },
        "wsSettings": {
          "path": "/",
          "headers": {}
        }
      },
      "mux": {
        "enabled": false,
        "packetEncoding": "xudp",
        "concurrency": -1
      }
    }
  ]
}
```