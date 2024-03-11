## Pass the Hash with Mimikatz

#### Resources <br/>
[What is Mimikatz?](https://www.varonis.com/blog/what-is-mimikatz/)

---

Mimikatz is capable of various credential-gathering techniques, including pass-the-hash, pass-the-ticket, overpass-the-hash (pass-the-key), Kerberoasting for golden and silver tickets, and pass-the-cache attacks.
- Pass-the-hash: Mimikatz uses this method to use an NTLM hash as a means to authenticate to a target system without needing to know the plaintext password.
- Pass-the-ticket: This technique involves using a Kerberos ticket to authenticate as the ticket’s owner without requiring their password.

--

To safeguard against Mimikatz, we can limit administrative privileges, disable password caching, turn off debug privileges, and enhance Local Security Authority (LSA) protection. Limiting administrative privileges is crucial as Mimikatz requires elevated access to execute, so minimizing the number of users with such access inherently reduces the risk. Disabling password caching thwarts Mimikatz’s ability to retrieve authentication credentials from system memory, effectively blocking one of its primary attack pathways. These two mitigations directly target Mimikatz’s dependency on elevated access and its method of harvesting credentials from the system.