## Public Key Infrastructure (PKI)

*PKI, or Public Key Infrastructure, is like a digital passport system for the internet, verifying identities and establishing secure online communication. It's like a digital handshake that ensures when you're talking to a website, your information is kept private and secure.*

---
#### Three main components of PKI
**Certificate Authorities (CA):** These are trusted entities that issue and manage digital certificates.<br/>

**Registration Authorities (RA):** These assist in the verification of user identity before a CA issues a digital certificate.

**Digital Certificates:** These are electronic documents that use a digital signature to bind a public key with an individual's identity.

---
Imagine PKI as a system of digital ID cards for websites. When you visit a secure website (like online banking), PKI checks the website's ID card (digital certificate) to ensure it’s legitimate and not a fake. This process, happening in the background, protects the information you send to and receive from the website, keeping it safe from eavesdroppers.

---
The **primary weakness in PKI** is the dependency on the trustworthiness of the Certificate Authorities. If a CA is compromised or behaves maliciously, it can issue fraudulent certificates, potentially undermining the security of the entire system.

#### Resources
[What is Public Key Infrastructure (PKI)](https://www.ssh.com/pki/)