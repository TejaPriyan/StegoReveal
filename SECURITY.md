# Security Policy

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 1.0.x   | :white_check_mark: |

## Security & Architecture Model

**StegoReveal** is engineered as a **Zero-Knowledge, Client-Side Application**:
1. **Zero Server Transmission**: Carrier images, decoded bytes, and passwords are never transmitted to any remote server or third party. All computation runs inside your local browser runtime.
2. **Cryptographic Standards**:
   - Primary: Web Crypto API (Hardware-accelerated AES-256-GCM, PBKDF2-HMAC-SHA256 with 100,000 rounds).
   - Fallback: Pure-JS FIPS 197 / NIST SP 800-38D compliant cipher suite for constrained environments.
   - Integrity: IEEE 802.3 CRC32 verification prior to payload delivery.

## Reporting a Vulnerability

If you discover a security vulnerability in StegoReveal:
1. Please do **NOT** open a public issue.
2. Email details to: `teja1616150@gmail.com`.
3. Include:
   - Description of the vulnerability.
   - Steps to reproduce or proof-of-concept carrier image.
   - Potential impact analysis.

We strive to respond within 48 hours and release patches promptly.

