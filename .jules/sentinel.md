## 2026-11-05 - [CRITICAL] Supply Chain Vulnerability in polyfill.io
**Vulnerability:** Use of `polyfill.io` which has known supply chain vulnerabilities (domain was sold and started serving malicious code).
**Learning:** Third-party CDNs for core features can become compromised. The `polyfill.io` service was a major supply chain attack vector.
**Prevention:** Avoid using `polyfill.io`. Use secure alternatives like `cdnjs.cloudflare.com/polyfill` or bundle polyfills directly.
