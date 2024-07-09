# Investigating-with-splunk (Tryhackme:SOC Level 1)


<H2>Description</H2>
This is a hands-on project on SIEM making use of Splunk.
<br/>

<h2>Unilities Used</h2>
-<b>Splunk Enterprise</b>

<h2>Enviroments Used</h2>
-<b>Tryhackme Virtual Machine</b>

<h2>Walk-through</h2>
<h3><b>Questions</b></h3>
<img src="https://i.imgur.com/uOI9O7t.png" height="80%" width="80%" alt="Investigating with splunk"/>
<img src="https://i.imgur.com/OpIXu0C.png" height="80%" width="80%" alt="Investigating with splunk"/>

<h3>Here are the steps taken to solve the Problems</h3>

Q1. Finding the Number of events in splunk
<img src="https://i.imgur.com/VOnkcdH.png" height="80%" width="80%" alt="Investigating with splunk"/>
<br>

Q2. Figuring out the new Username?

<img src="https://i.imgur.com/zpNJat2.png" height="80%" width="80%" alt="Investigating with splunk"/>
I searched for the EventID to discover sucessfully created Backdoorwhich was used in the Splunk Search to find the answer.

<img src="https://i.imgur.com/SqZUNfG.png" height="80%" width="80%" alt="Investigating with splunk"/>

Q3. Finding the full path regisry key of the backdoor of the new User?

<img src="https://i.imgur.com/Lu0Q0sH.png" height="80%" width="80%" alt="Investigating with splunk"/>

Q4. Which user was impersonated? 

<img src="https://i.imgur.com/34kSXEr.png" height="80%" width="80%" alt="Investigating with splunk"/>

Q5. Command Used to add the back door?
<img src="https://i.imgur.com/FKWBDWt.png" height="80%" width="80%" alt="Investigating with splunk"/>
Using the EventID 4688 to find the newly created backdoor.

Q6. How many times login attempt from the backdoor was observed?
Using the EventID 4625 to find the number of login attempts
<img src="https://i.imgur.com/UohLInp.png" height="80%" width="80%" alt="Investigating with splunk"/>

Q7. What is the name of the infected host on which suspicious power shell command were executed?
<img src="https://i.imgur.com/mPPeEs5.png" height="80%" width="80%" alt="Investigating with splunk"/>

Q8. How many malicious Powershell command were executed?
Using the eventID 4103 to find out Malicious Powershell command
<img src="https://i.imgur.com/8e7BAh0.png" height="80%" width="80%" alt="Investigating with splunk"/>

Q9. Find the encoded Powershell scriptnfrom the infected Host . what is the full URL?
<br>
Finding the encoded script

<img src="https://i.imgur.com/ouxf62Y.png" height="80%" width="80%" alt="Investigating with splunk"/>

Decoding the encoded Base64 text from splunk
<img src="https://i.imgur.com/TxCSzTY.png" height="80%" width="80%" alt="Investigating with splunk"/>

Decoding the encoded Base64 text from the previous decoded text
<img src="https://i.imgur.com/gibRkG7.png" height="80%" width="80%" alt="Investigating with splunk"/>

Defanging the decoded text to get the full URL
<img src="https://i.imgur.com/MsfIcEX.png" height="80%" width="80%" alt="Investigating with splunk"/>

<h2>ANSWERS</h2>
<img src="https://i.imgur.com/SN01rkl.png" height="80%" width="80%" alt="Investigating with splunk"/>

