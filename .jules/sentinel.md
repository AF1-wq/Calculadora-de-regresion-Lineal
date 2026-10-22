## 2023-10-22 - [CRITICAL] Supply Chain Attack via polyfill.io
**Vulnerability:** The application was loading scripts directly from `polyfill.io`, a domain that has been acquired by an untrusted entity and used to serve malicious JavaScript (supply chain attack).
**Learning:** External dependencies, especially CDNs for scripts that execute in the client's browser, pose a significant supply chain risk if the domain changes ownership or is compromised. Trusting third-party CDNs blindly is a critical security vulnerability.
**Prevention:** Use trusted, well-established CDNs (like Cloudflare's cdnjs or jsDelivr), implement Subresource Integrity (SRI) where possible, or bundle dependencies locally instead of relying on external URLs for critical assets.
