## 2024-06-25 - [Supply Chain] polyfill.io Domain Hijacking
**Vulnerability:** The `polyfill.io` domain was sold to a new entity and subsequently observed injecting malware/redirects into scripts requested from it, creating a critical supply chain vulnerability for any site loading it.
**Learning:** Hardcoded, un-subresource-integrity (SRI) verified third-party script tags (especially from free generic CDNs) introduce immense supply chain risk if domain ownership changes.
**Prevention:** Use trusted CDNs (like Cloudflare's cdnjs mirror for polyfill), always use Subresource Integrity (SRI) hashes when loading external scripts, and prefer self-hosting critical dependencies or bundling them.
