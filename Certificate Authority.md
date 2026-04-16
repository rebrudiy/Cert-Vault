---
tags: [concept, cryptography, certificates]
aliases: [CA, root CA, intermediate CA]
---

# Certificate Authority (CA)

## Definition

**Certificate Authority (CA)** — a trusted entity that issues and signs digital certificates. It vouches that a public key belongs to a specific person/organization.

**Root CA** — the top-level CA in a PKI hierarchy. Its certificate is self-signed — it trusts itself. All other certificates in the chain trace back to it.

## Types of CAs

### Intermediate CA

### Private CA

## How a CA Issues a Certificate

## Trust Store

> [!todo]
> - How authorized CAs get their certificates into browsers/OS trust stores
> - How deprecated/compromised CA certs are removed and replaced

## Risks

## Related
- [[Certificate Chain]]
- [[PKI]]
- [[X.509 Certificate]]
- [[Certificate Revocation]]
