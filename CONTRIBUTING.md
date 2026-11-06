# Contributing to StegoReveal

Thank you for your interest in contributing to **StegoReveal**! We welcome bug reports, algorithm improvements, user experience enhancements, and documentation updates.

## Code of Conduct

This project adheres to the Contributor Covenant Code of Conduct. By participating, you are expected to uphold this code. Please read [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for details.

## How Can I Contribute?

### 1. Reporting Bugs
- Search existing issues before creating a new one.
- Use the **Bug Report** template.
- Provide carrier image specifications (dimensions, format: PNG/WEBP/JPG) and browser details.
- Never attach confidential or sensitive messages.

### 2. Suggesting Enhancements
- Open a feature request issue describing the enhancement.
- Discuss cryptographic and steganographic implications if applicable.

### 3. Submitting Pull Requests
1. Fork the repository on GitHub.
2. Clone your fork locally:
   ```bash
   git clone https://github.com/<your-username>/StegoReveal.git
   cd StegoReveal
   ```
3. Create a descriptive branch:
   ```bash
   git checkout -b feature/robust-stego-decoder
   ```
4. Test all changes across major browsers (Chrome, Firefox, Safari, Edge).
5. Verify that Web Crypto API and pure-JS fallback execute smoothly without regressions.
6. Commit with clear, descriptive commit messages.
7. Push to your fork and submit a Pull Request.

## Security Considerations

Because StegoReveal implements cryptographic operations (PBKDF2-HMAC-SHA256, AES-256-GCM) and pixel extraction, all cryptographic logic must:
- Adhere to NIST SP 800-38D and RFC 8018 standards.
- Maintain zero-server data leak guarantees (100% in-browser processing).
- Never send carrier pixels or decrypted plaintext over any network channel.
