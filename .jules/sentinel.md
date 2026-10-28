## 2024-05-24 - [CRITICAL] polyfill.io Supply Chain Vulnerability
**Vulnerability:** The `index.html` file was using a script from `polyfill.io`. This domain was sold and has been caught serving malicious code in a massive supply chain attack.
**Learning:** External CDNs for seemingly harmless polyfills can become critical attack vectors if the domain changes hands or gets compromised.
**Prevention:** Avoid using `polyfill.io`. Use trusted alternatives like `cdnjs.cloudflare.com/polyfill` or bundle polyfills directly during the build process if possible.
