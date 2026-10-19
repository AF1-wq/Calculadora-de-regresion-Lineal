## 2024-03-24 - [Remove Malicious Polyfill.io Script]
**Vulnerability:** The codebase included a script tag pointing to `polyfill.io`. This domain was compromised in a supply chain attack and serves malicious code to users.
**Learning:** Third-party dependencies loaded via CDN are susceptible to supply chain attacks if the domain is sold or compromised. Using unpinned/untrusted external resources introduces significant risk.
**Prevention:** Avoid using unnecessary external scripts. If a CDN must be used, use a reputable one (like cdnjs, jsdelivr) and always include Subresource Integrity (SRI) attributes. Modern browsers rarely need polyfills like this anymore.
