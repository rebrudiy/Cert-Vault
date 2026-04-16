---
tags:
  - concept
  - cryptography
  - certificates
  - protocols
  - "network"
aliases:
  - TLS
  - SSL handshake
---
# TLS Handshake

## Definition

**Transport Layer Security (TLS)** is a cryptographic protocol designed to provide communications security over a computer network, such as the Internet. It is widely used in applications such as email, instant messaging, and voice over IP, but its use in securing HTTPS remains the most publicly visible.


## Resources

- [TLS 1.3 step by step introduction](https://tls13.xargs.org/)



## TLS 1.3 Handshake Flow

**Client step 1** *key generation*
- Generates 32-byte private key using [[X25519]] algorithm
- Derives public key from private key

> [!example]+
> ```
> ### requires openssl 1.1.0 or higher
> $ openssl pkey -noout -text < client-ephemeral-private.key
>
> X25519 Private-Key:
> priv:
> 20:21:22:23:24:25:26:27:28:29:2a:2b:2c:2d:2e:2f:30:31:32:33:34:35:36:37:38:39:3a:3b:3c:3d:3e:3f
>
> pub:
> 35:80:72:d6:36:58:80:d1:ae:ea:32:9a:df:91:21:38:38:51:ed:21:a2:8e:3b:75:e9:65:d0:d2:cd:16:62:54
> ```
> - *private_key* = `20:21:22:23:24:25:26:27:28:29:2a:2b:2c:2d:2e:2f:30:31:32:33:34:35:36:37:38:39:3a:3b:3c:3d:3e:3f`
> - *public_key* = `35:80:72:d6:36:58:80:d1:ae:ea:32:9a:df:91:21:38:38:51:ed:21:a2:8e:3b:75:e9:65:d0:d2:cd:16:62:54`

**Client step 2** *Client Hello*
- client random data
- a list of cipher suites that the client supports
- a list of public keys that server might find suitable for key exchange
- protocol versions that the client can support

| number           | explanation   |
| ---------------- | ------------- |
| `16 03 03 00 7a` | record header |
|                  |               |

## Certificate's Role

## Key Agreement

## TLS 1.2 vs TLS 1.3

## Prerequisites
- [[Digital Signatures]]
- [[X.509 Certificate]]
- [[Certificate Chain]]

## Related
- [[Certificate Types]]
- [[Certificate Revocation]]
