## 2026-11-10 - [CRITICAL] Supply Chain Vulnerability in polyfill.io
**Vulnerability:** The domain `polyfill.io` was sold and has been serving malicious code. It's a known, critical supply chain vulnerability for any site loading scripts from it.
**Learning:** Loading third-party scripts from untrusted or recently sold domains can compromise the entire frontend, leading to XSS and data theft.
**Prevention:** Avoid using `polyfill.io`. Use trusted alternatives like `cdnjs.cloudflare.com/polyfill` for polyfills, and implement Subresource Integrity (SRI) where possible.
