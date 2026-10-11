## 2024-07-01 - Compromised CDN Domain (Polyfill.io)
**Vulnerability:** The application was loading a script from polyfill.io, a domain that was sold and has been caught serving malicious code in a massive supply-chain attack.
**Learning:** External dependencies, especially those loaded via CDN without Subresource Integrity (SRI) hashes, can become malicious over time if the domain changes ownership or is compromised.
**Prevention:** Avoid unmaintained/sold CDN domains. Use reputable CDNs (like cdnjs, jsdelivr) and always include Subresource Integrity (SRI) hashes for external scripts.
