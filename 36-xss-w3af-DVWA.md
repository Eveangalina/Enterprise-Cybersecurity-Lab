## XSS with w3af, DVWA
#### Resources <br/>
[Cross-site scripting](https://portswigger.net/web-security/cross-site-scripting) <br/>
[Security Report for In-Production Web Applications](https://www.rapid7.com/globalassets/_pdfs/whitepaperguide/rapid7-tcell-application-security-report.pdf) <br/>

---

**Explain how a cross-site scripting attack works in non-technical terms.**

Cross-site scripting (XSS) is a web security vulnerability that allows attackers to compromise the interactions users have with a vulnerable application. It enables attackers to circumvent the same-origin policy, which segregates different websites from each other. XSS vulnerabilities typically allow an attacker to act as a victim user, to perform actions the user can do, and to access the user's data. If the user has privileged access, the attacker may gain full control over the application's functionality and data. 

---

**What are the three types of XSS attacks?**

**Stored XSS:** This is like someone putting that bad note into a library book. You check out the book, read the note, and the mischief happens. <br/>
**Reflected XSS:** This one is like getting a flyer that has a mischievous note written on the back. When you read the flyer and turn it over, you get tricked into the chaos. <br/>
**DOM-based XSS:** Think of this as someone telling you a riddle that changes the way you understand the words. When you solve the riddle, you end up doing something you didn't intend to do.

---

**If an attacker successfully exploits a XSS vulnerability, what malicious actions would they be able to perform?**

If a hacker pulls off an XSS attack, they can do a variety of naughty things. They can pretend to be you on the website, do things you can do, see your private info, and even control the website if they're really sneaky. Imagine someone using a fake ID to access your gym locker, workout as you, and swipe your personal stuff.

---

**What are some security controls that can be implemented to prevent XSS attacks?**

Content Security Policy (CSP): A security measure that helps detect and mitigate certain types of attacks, including XSS and data injection attacks. By specifying valid sources of content, CSP prevents the browser from loading malicious assets.<br/>

Input Sanitization: Ensuring that user input is checked and cleansed before it's processed by the application can prevent malicious scripts from being injected. <br/>

Output Encoding: When displaying user input, the application should encode the output, turning potentially dangerous characters into harmless encoded representations. <br/>

Use of Frameworks: Modern development frameworks often have built-in mechanisms to automatically escape user input and protect against common web vulnerabilities. <br/>

Regular Security Audits: Conducting security reviews and penetration testing can help identify and remediate XSS vulnerabilities before attackers can exploit them.<br/>

Educating Developers: Developers should be trained to understand XSS vulnerabilities and how to prevent them. Knowledge of secure coding practices is vital.<br/>

Updating and Patching: Keeping software up to date with the latest security patches can protect against known vulnerabilities that might be exploited via XSS. <br/>


These controls are fundamental in creating a robust defense against cross-site scripting attacks.