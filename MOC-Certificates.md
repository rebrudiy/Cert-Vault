# MOC - Certificates

> Entry point for everything related to digital certificates, PKI, and TLS.

---

## 🗺️ Learning Roadmap

### Stage 1 — Foundations (start here)
Prerequisites before touching certificates:
- [[Digital Signatures]] — how signing works mathematically
- Basic asymmetric crypto (public/private key pairs)
- Hash functions (SHA-256, etc.)

### Stage 2 — Certificate Basics
- [[X.509 Certificate]] — what a certificate actually is
- [[Certificate Authority]] — who issues and signs certificates
- [[Certificate Chain]] — how trust flows from root to end-entity

### Stage 3 — PKI (the whole system)
- [[PKI]] — Public Key Infrastructure, the full ecosystem
- [[Certificate Revocation]] — CRL, OCSP, what happens when certs go bad
- Certificate lifecycle: issuance → renewal → revocation

### Stage 4 — Certificate Types
- [[Certificate Types]] — DV, OV, EV, Wildcard, SAN, mTLS client certs
- Code signing certificates
- Email certificates (S/MIME)

### Stage 5 — TLS (certificates in action)
- [[TLS Handshake]] — how certificates are used in TLS
- TLS 1.2 vs TLS 1.3 differences
- SNI (Server Name Indication)
- Certificate pinning

### Stage 6 — Formats & Tooling
- [[Certificate Formats]] — PEM, DER, PKCS#7, PKCS#12
- OpenSSL — create, inspect, verify certs
- Let's Encrypt / ACME protocol
- Creating self-signed certificates

### Stage 7 — Advanced
- Certificate Transparency (CT logs)
- CAA DNS records
- DANE / TLSA
- [[mTLS]] — mutual TLS, both sides authenticate

---

## 📚 All Notes

### Core Concepts
- [[X.509 Certificate]]
- [[Certificate Authority]]
- [[Certificate Chain]]
- [[Digital Signatures]]
- [[PKI]]

### Lifecycle & Trust
- [[Certificate Revocation]]
- [[Certificate Types]]

### In Practice
- [[TLS Handshake]]
- [[Certificate Formats]]

---

## 🔗 Related MOCs
- [[MOC-Crypto]] — broader cryptography context
- TLS 1.3 — see vault root note
