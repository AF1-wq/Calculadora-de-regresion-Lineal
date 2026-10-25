## 2026-10-25 - Supply Chain Attack via polyfill.io
**Vulnerability:** The application was loading scripts directly from `polyfill.io`, a domain that was sold and has been observed serving malware (supply chain attack).
**Learning:** External CDNs for seemingly benign resources (like polyfills) can be compromised or change ownership, leading to immediate critical vulnerabilities if SRI or safe mirrors are not used.
**Prevention:** Use trusted, verified CDNs (like `cdnjs.cloudflare.com`) or host resources locally. Implement Subresource Integrity (SRI) for external scripts where applicable.
