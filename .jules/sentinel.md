## 2024-05-15 - [polyfill.io Supply Chain Vulnerability]
**Vulnerability:** Use of polyfill.io script which has known supply chain vulnerabilities after changing ownership.
**Learning:** External dependencies, especially CDNs, can become malicious if ownership changes. Relying on scripts from untrusted domains allows them to inject arbitrary code (XSS).
**Prevention:** Avoid polyfill.io. Use trusted, secure alternatives like cdnjs.cloudflare.com/polyfill. Always verify the trustworthiness of external script sources.