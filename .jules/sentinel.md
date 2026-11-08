## 2024-03-24 - [Supply Chain] Polyfill.io Domain Hijacking Vulnerability
**Vulnerability:** The domain polyfill.io was sold and has been serving malicious code to users, creating a severe supply chain attack vulnerability for any site loading scripts from it.
**Learning:** External CDNs for scripts can become malicious if the domain changes ownership or is compromised. Trusting third-party domains unconditionally is a risk.
**Prevention:** Use reliable, trusted CDNs like cdnjs or host dependencies locally when possible. Always verify the integrity and ownership of third-party script sources.
