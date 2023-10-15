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

<p align="center">
<br/>
<img src="https://imgur.com/HscNIdy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
<br/>
<img src="https://imgur.com/vzSJpJJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
<br/>
<img src="https://imgur.com/aYiHelF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
<br/>
<img src="https://imgur.com/J5Ryyji.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
<br/>
<img src="https://imgur.com/3EcCsPK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
<br/>
<img src="https://imgur.com/vhApfT5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
<br/>
<img src="https://imgur.com/lPbjelK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<p align="center">
<br/>
<img src="https://imgur.com/30ojWok.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<h2>Discussion of the Key Findings from the T-Pot Honeypot</h2>
- Total number of attacks on the honeypots amounted to 121,346 for 5 days.
<br>
<br>
- Top honeypots attacked were Ddospot (DDOS attacks), Dionaea (network attacks with malware), Cowrie (brute force attacks with SSH and Telnet), and Honeytrap (TCP & UDP service attacks).
<br>
<br>
- Top ports attacked were port 123 (NTP), port 21 (FTP), port 443 (HTTPS), port 53 (DNS), and port 22 (SSH).
<br>
<br>
- Top countries attacking the honeypots are the United States, Argentina, Brazil, China, and India.
<br>
<br>
- Top Suricata alerts are attempting denial of service and detection of a network scan.
<br>
<br>
- Top attempted usernames are root, admin, user, sa (sql database admin), guest, and test.
<br>
<br>
- Top attempted passwords letmein, jordan, 1234, admin, 123456, master 160887, and 1qaz@WSX.
<br>
<br>
This information can be used to harden and defend an organization's network.  I suspected most of the attacks would be on the network.  It seemed as though the attackers tried to penetrate the network.  There were malicious files dropped onto the honeypots.  There is a list of the top 10 malware samples dropped.  I could take those samples and upload them to a sandbox to analyze.  The analysis of the malware could be another project idea for the future.
<br>
<br>
If you have any more questions about the data, feel free to email me at robert.d.russ@proton.me.
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
