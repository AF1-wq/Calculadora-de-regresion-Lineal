## 2025-01-20 - [CRITICAL] Supply Chain Vulnerability in polyfill.io
**Vulnerability:** The application was loading a script from `polyfill.io`, a domain that was sold to a new entity and is known to be involved in a significant supply chain attack. Loading scripts from this domain can allow attackers to execute arbitrary malicious code on users' machines.
**Learning:** External dependencies, especially CDNs providing JavaScript files, can be compromised or sold to malicious actors. `polyfill.io` was a known, trusted service that became a vector for malware. It's crucial to use trustworthy, maintained, and secure CDNs (like `cdnjs.cloudflare.com`) or bundle dependencies locally when possible.
**Prevention:**
1. Use secure and trusted alternatives for polyfills, such as `cdnjs.cloudflare.com/polyfill`.
2. Keep abreast of security advisories related to third-party dependencies and CDNs.
3. Consider using Subresource Integrity (SRI) attributes for scripts loaded from external sources.
4. If feasible, bundle dependencies instead of relying on external CDNs.
