## Cloud Identity and Access Management (IAM) with AWS

#### Resources
[Lessons Learned from the Capital One Data Breach (PDF)](https://www.zscaler.com/resources/white-papers/capital-one-data-breach.pdf)

----

So, diving into that PDF, the three commands that the attacker used were:

- A command to get the security credentials for the WAF-Role using a Server-Side Request Forgery (SSRF) attack to call the metadata service of an EC2 instance.

- A command to list all the S3 buckets accessible with the WAF-Role.

- A command to sync and download the data from the S3 buckets they had listed​
---
The attack was possible because of a *misconfigured Web Application Firewall (WAF)* that allowed the attacker to access the metadata service endpoint using SSRF. This misconfiguration, combined with excessive permissions assigned to the IAM role, allowed the attacker to list and download data from the S3 buckets. 

---
A couple of governance strategies within AWS that may have averted the breach include:

- Conducting thorough audits of access channels and privileges granted to both users and automated services regarding data repositories like S3 buckets. Implementing CIEM tools could have been crucial in spotting any instances where permissions were too lax or data was unnecessarily vulnerable.
- The deployment of CSPM tools to streamline the enforcement of security and regulatory frameworks could also have been key. This includes mandating the adoption of the updated and more secure EC2 Metadata service version 2 over the older version 1.