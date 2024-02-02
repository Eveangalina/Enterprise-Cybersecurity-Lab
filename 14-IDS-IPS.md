### Intrusion Detection and Prevention Systems (IDS/IPS)
*Two differences between firewalls and an Intrusion Detection System (IDS) are:*

**Traffic Control vs. Monitoring:** <br/>
<u>Firewall:</u> It acts as a barrier to control which traffic can enter or leave a network based on predetermined security rules.

<u>IDS:</u> It monitors and analyzes network traffic for suspicious activities and signs of attacks but does not block traffic by itself.


**Visibility Level:** <br/>
<u>Firewall:</u> Operates predominantly at the network and transport layers, examining packet headers and state information to make allow-or-deny decisions. <br/>

<u>IDS:</u> Works at a higher level, inspecting the content of traffic (payload) to identify patterns or signatures indicative of attacks.

---

A network-based IDS is preferred when you need to safeguard the entire network's infrastructure, as it allows for the inspection and analysis of the collective traffic flowing through the network. This contrasts with a host-based system that protects individual devices. 

A NIDS is particularly useful for identifying threats that are not targeted at a single host but could affect the entire network.

---
**Three major drawbacks of a NIDS are:**

**Limited Visibility:** NIDS can struggle to analyze encrypted traffic, which means threats concealed within encrypted packets might go undetected. <br/>

**Resource Intensive:** They can require significant processing power to analyze all network traffic, leading to potential performance bottlenecks.<br/>

**False Positives/Negatives:** NIDS can generate false alarms, mistaking normal activities for threats, or they may fail to detect some sophisticated attacks, leading to false negatives.


#### Resources 
[The Pros and Cons of Network Intrusion Detection Systems](https://blog.rapid7.com/2017/01/11/the-pros-cons-of-intrusion-detection-systems/)