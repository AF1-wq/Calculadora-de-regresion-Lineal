## 2026-11-03 - [CRITICAL] Supply Chain Vulnerability via polyfill.io
**Vulnerability:** The application was loading scripts from `polyfill.io`, which is a known supply chain vulnerability due to the domain being acquired by a potentially malicious actor. This could lead to arbitrary JavaScript execution in the user's browser (XSS).
**Learning:** Third-party CDNs and script providers can change ownership or be compromised. Relying on them blindly, especially those that serve dynamic scripts based on user-agent, introduces significant risk.
**Prevention:** Avoid using `polyfill.io`. Use secure, reputable alternatives like `cdnjs.cloudflare.com/polyfill` or host dependencies locally where feasible. Use Subresource Integrity (SRI) when loading scripts from CDNs.
