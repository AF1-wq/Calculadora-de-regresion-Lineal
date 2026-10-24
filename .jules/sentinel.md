## 2024-05-24 - [Supply Chain] polyfill.io Compromise
**Vulnerability:** The `polyfill.io` domain was sold and modified to serve malicious code (supply chain attack). Applications including it directly are vulnerable to XSS and arbitrary code execution in the browser.
**Learning:** Using third-party CDN scripts without Subresource Integrity (SRI) or from untrusted maintainers creates a critical supply chain vulnerability.
**Prevention:** Use trusted CDNs (like Cloudflare's mirror `cdnjs.cloudflare.com/polyfill`), use self-hosted scripts where possible, or pin versions with SRI hashes.
