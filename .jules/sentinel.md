## 2024-05-23 - [Critical] Compromised polyfill.io CDN Domain
**Vulnerability:** The `index.html` file included a script from `polyfill.io`. This domain was sold and subsequently started serving malicious code in a massive supply-chain attack.
**Learning:** Using third-party CDNs introduces a supply-chain risk. Even reputable domains can change ownership or be compromised.
**Prevention:**
1. Prefer hosting dependencies locally when possible.
2. If using CDNs, use Subresource Integrity (SRI) hashes to ensure the file contents haven't been tampered with.
3. Keep track of security news regarding dependencies and services used in the project.
4. Specifically for polyfill.io, use safe mirrors like Cloudflare's `cdnjs` or Fastly's `polyfill.io` fork.
