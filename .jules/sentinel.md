## 2024-11-06 - [CRITICAL] Supply Chain Vulnerability in polyfill.io
**Vulnerability:** The `index.html` file was referencing `https://polyfill.io/v3/polyfill.min.js`. The `polyfill.io` domain was sold and the new owner has been known to inject malicious code (supply chain attack) into the script based on the referring site, potentially executing arbitrary JavaScript on users' browsers.
**Learning:** External dependencies, especially scripts loaded from a CDN, present a significant supply chain risk. Relying on domains that can change ownership or be compromised without notice can instantly compromise the application.
**Prevention:**
1. Use trusted, widely recognized CDNs (like `cdnjs` or `jsdelivr`) instead of single-purpose domains that may be sold.
2. For critical scripts, always use Subresource Integrity (SRI) hashes to ensure the file fetched matches the expected content.
3. Where feasible, host polyfills and dependencies locally rather than relying on external CDNs.
