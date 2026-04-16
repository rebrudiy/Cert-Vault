---
tags:
  - concept
  - cryptography
  - certificates
  - mathematics
aliases:
  - digital signature
  - signing
---

# Digital Signatures

## Definition
**CMS (Cryptographic Message Syntax)** — a standard format (PKCS#7) for signed/encrypted data. When you sign a document with OpenSSL, the output is a CMS file containing the document + signature + signer's certificate.

**Digital Signature** — a cryptographic mechanism that proves the authenticity and integrity of a message or document. It guarantees that the data was signed by a specific private key holder and was not modified after signing.

## How It Works

### Certificate Issuance

**User:**
- Generate private and public key
- Create file with his name and public key
- Encrypt file hash with private key
- Send file + encrypted hash to CA

**CA:**
- Gets user data
- Validates that with public key can decrypt hash
- Generate certificate with user info + public key, sign it with its private key

### Signing
- Encrypt document hash with private key
- Send certificate + document + encrypted hash to other user

### Verification
- Check that with public key the encrypted hash can be decrypted
- Check that certificate is valid and not revoked

## Properties

## Common Algorithms

## Role in Certificates

## Related
- [[X.509 Certificate]]
- [[Certificate Authority]]
- [[PKI]]
