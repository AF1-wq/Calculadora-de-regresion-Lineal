## 2024-06-25 - Supply Chain Attack via `polyfill.io`
**Vulnerability:** The application was using the `polyfill.io` service directly from the official domain. In June 2024, the `polyfill.io` domain was sold and the new owners were observed injecting malicious code into the responses served to websites, executing a supply chain attack that could compromise end users.
**Learning:** External dependencies, even commonly used CDNs, can become compromised if the domain changes ownership or the service is breached. We implicitly trusted a domain without using Subresource Integrity (SRI) or relying on more strictly governed CDNs.
**Prevention:**
1. Use trusted, widely governed CDNs like `cdnjs.cloudflare.com` or self-host critical dependencies.
2. Consider using Subresource Integrity (SRI) hashes when loading external scripts if the URL provides a versioned, static file.
3. Be aware of security advisories related to third-party services and domains.