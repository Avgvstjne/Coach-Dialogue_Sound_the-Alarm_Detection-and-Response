# Coach-Dialogue_Sound_the-Alarm_Detection-and-Response
---

[Incident Handler's Journal entries](./docs/Incident-handlers-journal-several-entries.pdf)

---

Augustine   
Let's get started

Coach   
Great! Let's start by discussing foundational network security technologies. These are the tools used at the edge of a network to protect it from external threats. Can you identify and describe some of these technologies, such as firewalls, intrusion detection/prevention systems (IDS/IPS), or secure gateways like VPNs?

Augustine   
Can you please rephrase the question?

Coach   
Of course! Let's simplify that. When we talk about protecting a network from the outside world, what are some basic security tools or systems that come to mind? Think about things that act like a gatekeeper or a guard at the entrance of a network. What do they do?

Augustine   
We use IDS/IPS tools like Suricata to monitor intrusions, and SIEM tools like wazuh, splunk to monitor monitor our network and servers and have an overview of our data and event logs. We can use pfsense for firewall

Coach   
That's a great start! You've mentioned some excellent tools. Suricata for IDS/IPS is a good example of monitoring for intrusions, and you're right that SIEM tools like Wazuh and Splunk are crucial for overall network monitoring and log analysis. pfSense is indeed a popular choice for a firewall.

Now, let's dive a little deeper into the function of these foundational technologies. Can you explain what a firewall primarily does to protect a network from external threats?

Augustine   
FIrewall uses set rules to protect a network from unwanted traffic or access by blocking certain ports, or allowing only certain ports.

Coach   
Excellent! You've accurately described the core function of a firewall. It acts as a gatekeeper, using predefined rules to control incoming and outgoing network traffic, effectively blocking unwanted access and protecting against external threats.

Now, let's move on to Intrusion Detection/Prevention Systems (IDS/IPS). You mentioned Suricata earlier. Can you explain what an IDS/IPS does and how it differs from a firewall in its primary role of protecting the network?

Augustine   
An IDS works to detect an intrusion into a network then send out alerts notifying certain activities that it was set to notify. IPS on the other hand also has the characteristics of IDS only that IPS actually blocks access to the network when its set rules suggest an intrusion might be underway, then it sends alert. So, IDS sends alert to notify us of an intrusion while IPS actually blocks access. Both differ from firewall in the sense that they are sorta smarter because they inspect to make sure that the content of a package is actually safe not just the "labelling/addressing".

Coach   
That's a very clear and accurate distinction between IDS and IPS, and you've hit on a crucial point about how they differ from a firewall! You're right that IDS/IPS systems are "smarter" in that they inspect the content of network traffic, looking for malicious patterns or behaviors, rather than just the source, destination, or port.

Now, let's consider Secure Gateways, such as Virtual Private Networks (VPNs). How do VPNs contribute to securing a network, especially when users are accessing it from outside the physical perimeter?

Augustine   
VPNs secure a network by creating a private encrypted tunnel and provides an end-to-end encryption which scrambles data being transported and VPN also replaces IP addresses with its own thereby providing more security

Coach   
That's a fantastic explanation of how VPNs work! You've highlighted the key aspects: creating an encrypted tunnel, providing end-to-end encryption, and masking IP addresses. These features are indeed vital for securing remote access and protecting data in transit.

You've done a great job describing foundational network security technologies. Now, let's move on to Explore Internal Network Assets. Once traffic is inside the network perimeter, what technologies or strategies are used to protect internal assets and segments? Think about how we might limit movement within the network or control who can access what.

Augustine   
We can use IAM

Coach   
You're absolutely right that Identity and Access Management (IAM) is crucial for internal security! IAM helps control who can access what resources within the network. Can you elaborate a bit on how IAM, or perhaps other internal controls like network segmentation or Access Control Lists (ACLs), help limit lateral movement and protect sensitive data once a user is already inside the network?

Augustine   
IAM helps enforce least privilege and other management controls like MFAs so that if an attacker gains access through a user then that particular user's access can be blocked off until eradication is complete. But those controls also make it quite difficult for an attacker to easily move laterally and solidify their access to a network. Network segmentation also makes it difficult for an attacker to perform lateral movement, network segmentation is very useful to quarantine a particular part of a network that is under attack.

Coach   
That's an excellent explanation! You've clearly articulated how IAM, through principles like least privilege and multi-factor authentication (MFA), restricts an attacker's ability to move laterally even if they compromise a user account. And your description of network segmentation is spot on—it's a powerful way to contain threats and protect sensitive areas by isolating parts of the network.

Now, let's connect these concepts to real-world scenarios. We'll move on to Connect Network Security Threats to Technologies. Imagine a scenario where an attacker successfully breaches an external firewall and gains initial access to a network. What specific internal network security technologies or strategies would be most effective in detecting or preventing that attacker from moving deeper into the network to access sensitive data, and how would they work?

Augustine   
IDS/IPS tool like suricata would alert security personnel of the and of course the rules of IPS would have detected and stopped further movement into the network.

Coach   
You're absolutely right! An IDS/IPS like Suricata would be critical in this scenario. It would detect the suspicious activity of an attacker trying to move deeper into the network, and an IPS, specifically, could actively block that movement based on its rules. This highlights how internal IDS/IPS complements the perimeter defenses.

Now, let's consider another scenario: What if an attacker tries to exploit a known vulnerability in an internal web application to gain control? Which network security technology would be best suited to detect or prevent this kind of attack, and how would it help?

Augustine   
Wireshark would help detect this type of attack.

Coach   
Wireshark is an excellent tool for network analysis and can definitely help in investigating such an attack after it's happened, or even in real-time if you're actively monitoring. It allows you to see the raw network traffic.

However, for detecting or preventing an exploit against a web application vulnerability before it causes damage, another technology might be more directly suited. Can you think of a security technology specifically designed to protect web applications from attacks like SQL injection or cross-site scripting?

Augustine   
A Web Application Firewall protects web applications from attacks like SQL injection or cross-site scripting by filtering and monitoring HTTP traffic for malicious content.

Coach   
Exactly! A Web Application Firewall (WAF) is specifically designed for that purpose. It acts as a shield for web applications, inspecting HTTP traffic and blocking attacks like SQL injection and cross-site scripting before they can reach the application.

You've done a fantastic job connecting network security threats to the technologies designed to counter them. You've demonstrated a strong understanding of how various tools work together to protect a network.

Good job, you have completed all the topics for our session. Up next - view your feedback.

Coach   
During today's session covering describing common network security technologies and explaining their role in protecting network infrastructure and data, we focused on foundational network security technologies, internal network assets, and connecting threats to technologies.

Your strengths:

You demonstrate a clear understanding of the security technologies and their role in protection. You proactively explain and connect concepts, providing insightful descriptions of how the technologies function and interact.   
You consistently provided clear and accurate explanations, without needing continuous guidance from the coach.

Areas for improvement:

None. Your responses show you can describe network security technologies like a pro!   
Keep up the good work!
