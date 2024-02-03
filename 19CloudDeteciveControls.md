## Cloud Detective Controls

#### Reading
[What is Amazon GuardDuty?](https://docs.aws.amazon.com/guardduty/latest/ug/what-is-guardduty.html) <br/>
[AWS re:Inforce 2019: Threat Detection on AWS: An Introduction to Amazon GuardDuty (FND216)](https://www.youtube.com/watch?v=czsuZXQvD8E&ab_channel=AmazonWebServices)

**Amazon GuardDuty** can detect several Indicators of Compromise (IoCs) such as escalation of privileges, use of exposed credentials, communication with malicious IP addresses and domains, malware on Amazon EC2 instances and container workloads, unusual login patterns on databases, compromised EC2 instances and container workloads involved in activities like serving malware or bitcoin mining, and signs of AWS account compromise including unauthorized infrastructure deployments and unusual API calls. 

---

Amazon GuardDuty uses various data sources for its analysis, including VPC Flow Logs, AWS CloudTrail event logs (both management and S3 data event logs), and DNS logs. These sources enable GuardDuty to effectively monitor and identify suspicious activity within your AWS environment. 

---

GuardDuty analyzes access behavior by monitoring for unusual or unauthorized activities that deviate from established patterns. This includes detecting suspicious login attempts, such as logins from new geographic locations or the use of previously unseen IP addresses. By evaluating the context and characteristics of access events against known malicious signatures and anomalous activity patterns, GuardDuty identifies potential security issues or compromises.