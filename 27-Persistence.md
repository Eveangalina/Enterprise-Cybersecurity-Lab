### Persistence
---
**Major advantages of PowerShell Empire:** <br/>
PowerShell Empire's major advantage is its ability to leverage the PowerShell environment, which is a powerful scripting language built into Windows. 

It allows for the execution of a wide range of tasks on a host, such as gathering information, executing commands, and exfiltrating data, without needing to bring in external binaries that might trigger antivirus or intrusion detection systems. Its script-based nature makes it stealthy and versatile.

---

**APT groups known to use PowerShell Empire:**
Various *Advanced Persistent Threat* (APT) groups have been known to use PowerShell Empire, such as the **FIN7** cybercrime group and APT groups linked to nation-states.

These groups have utilized PowerShell Empire for activities like lateral movement within networks and executing code on compromised hosts. 

PowerShell Empire falls into several steps of the Cyber Kill Chain, including 'Command and Control' where it can communicate with a remote server to receive instructions, and 'Actions on Objectives' where the attacker uses it to achieve their end goal, such as data exfiltration or system compromise.

 * *FIN7, also known as Carbon Spider, ELBRUS, or Sangria Tempest, is a sophisticated Russian cybercrime group. Since mid-2015, they have primarily targeted the U.S. retail, restaurant, and hospitality sectors. They are known for using a front company called Combi Security to give a semblance of legitimacy to their operations. The group has been implicated in a variety of criminal activities, including spear-phishing campaigns and wide-scale breaches of financial data from companies, resulting in the theft of millions of customer credit and debit card numbers. They have been associated with several high-profile data breaches involving restaurants and other businesses.*

---
The four main components needed to pull off an attack using PS Empire are Listener, Agents, Modules, and Stager.

---

### Resources <br/>
[PowerShell Empire No Longer Maintained](https://www.bleepingcomputer.com/news/security/powershell-empire-framework-is-no-longer-maintained/) <br/>
[Hacking with Empire – PowerShell Post-Exploitation Agent](https://www.hackingarticles.in/hacking-with-empire-powershell-post-exploitation-agent/)