## 2024-10-20 - [CRITICAL] polyfill.io Supply Chain Vulnerability
**Vulnerability:** The `index.html` file was loading `polyfill.io`, a domain that was acquired by a Chinese company and subsequently observed serving malicious code (malware/redirects) in a large-scale supply chain attack.
**Learning:** External CDN dependencies can become compromised even if they were historically safe. Third-party domains represent a significant trust boundary.
**Prevention:** Use trusted, reputable CDNs (like cdnjs/Cloudflare) or bundle dependencies locally. Avoid unmaintained or recently sold domain resources. Ensure Subresource Integrity (SRI) is used where possible.
