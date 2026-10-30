## 2024-05-15 - [CRITICAL] polyfill.io Supply Chain Vulnerability
**Vulnerability:** The domain `polyfill.io` was sold and has been observed serving malicious code (supply chain attack). The application uses this domain to load polyfills.
**Learning:** Third-party domains (even CDNs) can be compromised or sold to malicious actors. Relying on them without integrity checks or subresource integrity (SRI) exposes the application to remote code execution / XSS via supply chain.
**Prevention:** Use a secure, well-known alternative CDN (like `cdnjs.cloudflare.com/polyfill`), use Subresource Integrity (SRI) when loading scripts, or bundle dependencies locally instead of loading them from external URLs.
