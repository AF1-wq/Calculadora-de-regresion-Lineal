## 2024-10-13 - [CRITICAL] polyfill.io supply chain attack
**Vulnerability:** The polyfill.io domain is used for legacy browser support but was recently compromised, resulting in it serving malicious code (a supply chain attack).
**Learning:** External dependencies, especially ones injected via `<script>` tags without Subresource Integrity (SRI) or from untrusted domains, can become vectors for severe attacks.
**Prevention:** Avoid third-party domains for polyfills when possible. If needed, self-host them or use a highly trusted, monitored CDN. For third-party scripts, always consider implementing Subresource Integrity (SRI) checks where applicable, and periodically audit all third-party resources.
