<h1>Tpot-Honeypot</h1>
Objective: To collect and analyze cyber threat intelligence to learn about potential threats.
<p align="center">
 <br/>
<img src="https://imgur.com/3XPwVF9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<h2>What is a honepot?</h2>
A honeypot is a cybersecurity mechanism designed to lure and deceive malicious actors. It involves setting up a decoy system or network with apparent vulnerabilities to attract potential attackers. The main purpose of honeypots is to gather cyber intelligence about their techniques, motivations, and tactics, allowing organizations to strengthen their security posture.
<br />

<h2>Why are honeypots important to an organization?</h2>
Honeypots are important to an organization for three key reasons and benefits: 
<br>
<br>
1. Early Threat Detection: They serve as a decoy to lure attackers, allowing the organization to identify and analyze threats before they reach critical systems. 
<br>
<br>
2. Threat Intelligence: By gathering data on attacker tactics and techniques, honeypots provide valuable insights that aid in improving overall cybersecurity defenses.
<br>
<br>
3. Vulnerability Assessment: Honeypots help identify weaknesses in the organization's security posture, enabling proactive measures to patch vulnerabilities and mitigate potential risks.

<h2>What are some downsides to having honeypots?</h2>
Some downsides to having honeypots include:
<br>
<br>
1. Resource Consumption: Honeypots require dedicated resources, both in terms of hardware and maintenance, which could impact an organization's budget and IT infrastructure.
<br>
<br>
2. False Positives: There is a risk of false positives, where legitimate users or automated scanners may inadvertently trigger the honeypot, leading to unnecessary alarms and distractions for security teams.
<br>
<br>
3. Increased Complexity: Managing honeypots adds complexity to an organization's cybersecurity infrastructure, and if not properly maintained, they could become an additional security risk if compromised by attackers.

<h2>Description of the T-Pot Honeypot</h2>
T-Pot is an open-source honeypot platform designed to emulate a diverse range of network services and systems to attract and trap potential attackers. Developed by Deutsche Telekom AG, T-Pot combines multiple honeypot tools into a single, integrated solution, making it easy to deploy and manage. It provides a wide variety of honeypot services, such as SSH, Telnet, HTTP, and more, offering attackers multiple entry points to interact with the decoy environment.

<h2>Implementation of the T-Pot Honeypot</h2>
To keep my environment safe, I decided to install a honeypot on a Debian VM on www.Vultr.com on a server in Dallas.  I followed the process laid out in the following YouTube video, https://youtu.be/TCTMR77c0dk.  Once the honeypot was installed, I let it run for several days to give it time to collect meaningful data.

<h2>Key Findings of the T-Pot Honeypot</h2>
<p align="center">
<br/>
<img src="https://imgur.com/jAtAI7S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<h2>IP Reputation Check</h2>
VirusTotal Risk Score: 0/87 vendors flagged IP as malicious.  The IP is clean.
<p align="center">
Hybrid Analysis Sandbox <br/>
<img src="https://imgur.com/EXz8vfD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />  
abuseIPDB Risk Score: IP address not found in database. The IP is clean.
<p align="center">
Hybrid Analysis Sandbox <br/>
<img src="https://imgur.com/nFzZnaP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />  

<h2>Declaration</h2>
This is a true positive because VirusTotal verified the attachment was malicious and the emails were delivered to the user’s inbox.

<h2>Recommendation(s)</h2>
I recommended the messaging team purge the emails from the user’s inbox and block the sender’s email address.
<img src="https://imgur.com/3XPwVF9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<p align="center">
Proofpoint Alert: <br/>
<img src="https://imgur.com/9fT3hBU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
