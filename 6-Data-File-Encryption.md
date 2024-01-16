# Data File Encryption
### Reading / Resources
- [Applying The CIA Triad To Your Enterprise File Transfer](https://www.jscape.com/blog/implementing-the-cia-triad-when-transferring-files-through-the-internet) <br/>

- [What Are MD5, SHA-1, and SHA-256 Hashes, and How Do I Check Them?](https://www.howtogeek.com/67241/htg-explains-what-are-md5-sha-1-hashes-and-how-do-i-check-them/)
- [ChatGPT](www.openai.com)

---
### <u>You have been made responsible for the company’s file server. How would you preserve the three elements of the CIA triad? </u>
I would preserve the three elements of the CIA triad in the following ways; 

- **Confidentiality**: I will implement encryption for both data at rest and in transit. To ensure that only authorized personnel have access, I'll use robust authentication mechanisms
- **Integrity:** I plan to employ hash functions and digital signatures to verify the authenticity and unaltered state of the data. I'll also conduct regular audits and integrity checks as they can be quite helpful
- **Availibility:** I will ensure redundancy through backups and failover systems. Additionally, I'll implement load balancing and enhance network resilience to handle peak demands and mitigate downtime risks.
---
#### <u>Explain how hashing verifies data integrity using non-technical terms.</u>

Think of a hash as a unique fingerprint for a file. Just like no two people have the same fingerprint, no two files have the same hash unless they are exactly identical. When you hash a file, you create its digital fingerprint. If the file changes even slightly, its hash changes completely. By comparing the hash of the received file with the original hash, you can tell if the file has been altered, thus verifying its integrity.

---
#### <u>How is hashing and encryption different?</u>
- Hashing converts data into a fixed-size string of charachters, which is typically a one-way process. Once data is hashed, you can't reverse it back to the original form
- Encryption transforms data into a secured form which can be reversed back to its original form using a key. It's a two-way process
