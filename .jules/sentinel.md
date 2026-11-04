## 2024-05-24 - [CRITICAL] Supply Chain Attack via polyfill.io
**Vulnerability:** The application was loading `polyfill.io` directly in `index.html`.
**Learning:** The `polyfill.io` domain was sold and has been caught serving malicious code in a supply chain attack affecting thousands of sites. This represents a critical risk of malicious code injection.
**Prevention:** Avoid using `polyfill.io`. Always use trusted, secure CDNs like `cdnjs.cloudflare.com/polyfill` for polyfills, or bundle polyfills directly during the build process if possible.
