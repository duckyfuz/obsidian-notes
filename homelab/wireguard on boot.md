- store the conf file in `/etc/wireguard/wg1.conf`
```
[Interface]
PrivateKey = XXX
Address = 10.74.66.2/24
DNS = 9.9.9.9, 149.112.112.112

[Peer]
PublicKey = XXX
PresharedKey = XXX
Endpoint = 34.45.161.86:51820
AllowedIPs = 0.0.0.0/0, ::0/0
```

- run `sudo systemctl enable wg-quick@wg1.service`

> [!tip] other useful commands
> `sudo systemctl start wg-quick@wg1.service`
> `sudo systemctl stop wg-quick@wg1.service`
> `sudo systemctl status wg-quick@wg1.service`
> `sudo systemctl disable wg-quick@wg1.service`
