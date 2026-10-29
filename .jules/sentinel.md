## 2026-10-29 - [CRITICAL] Supply Chain Vulnerability in polyfill.io
**Vulnerability:** The application was loading `polyfill.min.js` from `polyfill.io`. This domain was sold to a new entity and has been caught serving malicious code (supply chain attack), compromising any site using it.
**Learning:** External CDNs can become malicious if ownership changes. Relying on unverified third-party domains for executing JavaScript directly in the browser is a major supply chain risk.
**Prevention:** Avoid `polyfill.io` entirely. Use secure, reputable alternatives like `cdnjs.cloudflare.com/ajax/libs/polyfill/` or self-host dependencies.
