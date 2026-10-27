## 2024-11-20 - [Supply Chain] Compromised polyfill.io Domain Replacement
**Vulnerability:** The codebase was loading scripts directly from `polyfill.io`. The `polyfill.io` domain was sold to a malicious entity, and the CDN was observed serving malware and engaging in a massive supply chain attack affecting millions of sites. This represents a critical remote code execution (RCE) / Cross-Site Scripting (XSS) vulnerability.
**Learning:** External dependencies, especially CDNs providing Javascript, are a vector for supply-chain attacks. Even previously trustworthy domains can become malicious if ownership changes. Hardcoding such dependencies without integrity checks (SRI) leaves the application fully exposed to whatever the third party serves.
**Prevention:**
1. Migrate away from compromised CDNs (e.g., replace `polyfill.io` with secure alternatives like Cloudflare's mirror `cdnjs.cloudflare.com/polyfill`).
2. Use Subresource Integrity (SRI) attributes (`integrity="..."`) for all external scripts to ensure the loaded content matches the expected hash.
3. Where feasible, self-host dependencies rather than relying on external CDNs.