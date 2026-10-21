## 2025-02-14 - [Supply Chain Attack] Compromised CDN
**Vulnerability:** The application was loading a script from `polyfill.io`, a CDN that was recently acquired and is known to serve malware.
**Learning:** Relying on third-party CDNs introduces a supply chain risk. If the CDN is compromised or changes ownership, it can be used to inject malicious code into the application.
**Prevention:** Use reliable and trusted CDNs (like Cloudflare or unpkg) or host dependencies locally when possible. Always verify the integrity of external scripts using Subresource Integrity (SRI) hashes when available.
