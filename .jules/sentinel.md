## 2026-10-31 - [Supply Chain] Remove polyfill.io CDN
**Vulnerability:** The codebase uses `polyfill.io` which is known to be compromised and serves malicious code (supply chain attack).
**Learning:** Third-party CDNs, especially those that have changed ownership or have a history of compromise, can inject malicious scripts into the frontend application.
**Prevention:** Avoid `polyfill.io` entirely. Use secure, trusted alternatives like `cdnjs.cloudflare.com/polyfill` or host polyfills locally.
