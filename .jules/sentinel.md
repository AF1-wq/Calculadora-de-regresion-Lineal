## 2024-05-16 - [Supply Chain Vulnerability] polyfill.io
**Vulnerability:** Usage of `polyfill.io` which is known to be compromised in a supply chain attack.
**Learning:** Third-party scripts hosted on CDNs that change ownership or are compromised can serve malicious code to users without changing the script URL.
**Prevention:** Use trusted CDNs (like `cdnjs.cloudflare.com`), or host scripts locally. Avoid using services that are known to be vulnerable or unmaintained.
